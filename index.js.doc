/**
 * 1. Create a small method that you ask someone for a password which you know must
 *  be '123;, he has 3 chances, if he enters the password correctly, display 
 * "Continue" otherwise " You have been blocked"
 */

let chancesTried = 0
const validPass = '\'123;,'

const validatePass = function (pass) {
    chancesTried++
    const correctVldtMsg = 'Continue'
    const wrongVldtBlocked = 'You have been blocked'
    const wrongVldtMsg = 'Please try again'

    if (pass === validPass)
        return correctVldtMsg
    else if (chancesTried === 4) {
        chancesTried = 0
        return wrongVldtBlocked
    }
    else
        return wrongVldtMsg
};

console.log(validatePass())
console.log(validatePass())
console.log(validatePass())
console.log(validatePass())
console.log(validatePass(validPass))


/**
 * 2. Ask the end-user for a password, it must be 8 or more characters long, must contain 1 digit, one lowercase letter, 1 uppercase letter,
 *  1 special character. Check the password given, if it is valid, display "valid" otherwise display "invalid" and why
 */

const validatePass2 = (pass) => {
    let rtnMsg = 'invalid. '

    const digitRegex = /\d/g;

    const lowercaseRegex = /[a-z]/g

    const uppercaseRegex = /[A-Z]/g

    const specialCharRegex = /[!@#$%^&*()_+\-=\[\]{};':"\\|,.<>\/?]/

    if (pass.length < 8)
        rtnMsg += 'Your password must be 8 or more characters long'
    else if (!digitRegex.test(pass))
        rtnMsg += 'Your password must contain 1 digit'
    else if (!lowercaseRegex.test(pass))
        rtnMsg += 'Your password must contain one lowercase letter'
    else if (!uppercaseRegex.test(pass))
        rtnMsg += 'Your password must contain 1 uppercase letter'
    else if (!specialCharRegex.test(pass))
        rtnMsg += 'Your password must contain 1 special character'
    else rtnMsg = 'valid'

    return rtnMsg
}

console.log(validatePass2('aaaaaaaa22A'))
