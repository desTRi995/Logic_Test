# Logic-Test
Function Palindrome

#html
<form id="form_id">
    <input type="text" id="your_input" />
</form>

#javascriptpalindrome
var isPalindrome = function (string) {
    if (string == string.split('').reverse().join('')) {
        alert(string + ' is palindrome.');
    }
    else {
        alert(string + ' is not palindrome.');
    }
}

document.getElementById('form_id').onsubmit = function() {
   isPalindrome(document.getElementById('your_input').value);
    return false;
}
