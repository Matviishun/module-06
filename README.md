## JavaScript





function promptTest() {
    var name1 = prompt('Please, enter your name:');
    var name2 = prompt('Please, enter your name:',
                        'enter your name here...');
    print('Hello, ' + name1 + ' and ' + name2 + '!');
}

function confirmTest() {
    var name = prompt('Please, enter your name:');
    var isAdult = confirm('Are you adult?');
    print(name + (isAdult? ' is adult ' : ' is not ') + '!');
}


function ifElseTest() {
    var login = read('login');
    var password = read('password');
    print(login != '' && password != ''
        ? ('Login: ' + login + ', password: ' + password)
        : 'Please, enter login and password values');
    //admin login and password
    var adminLog = 'admin';
    var adminPass = 'admin';

    if (login != '' && password != '') {
        if (login == adminLog && password == adminPass) { // if true then ->
            /* -> */
            print('Hello, my Lord!&nbsp :)');
        } else {//if false then
            /* -> */
            print('Sorry, access denied');
        }
    }
}

function ternaryOperatorTest() {

    var a = read('a');
    var b = read('b');
    if (a == '' || b == '') {
        print('Some value was not received');
    } else {
        var min = +a < +b ? +a : +b;    //define with ternary operator and
                                        // comparison of a and b values
        var max = +a > +b ? +a : +b;    //define with ternary operator and
                                        // comparison of a and b values
        print('min: ' + min + '<br>max: ' + max);
    }
}

/*
* Task additor: *, /, +, -
 */
function additor() {
    var a = +(prompt("Please, enter 'a' number:"));
    var b = +(prompt("Please, enter 'b' number:",
                    'enter number here...'));
    print('a(' + a + ') + b(' + b + ') = ' + (a + b));
    
    
    link on project: https://matviishun.github.io/module-06/