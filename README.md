# goit-js-hw-02
Завдання 2:

//Друге рішення
// function formatMessage(message, maxLength) {
//     return message.length <= maxLength ? message : (message.slice(0, maxLength)) + "...";
// }
// console.log(formatMessage("Curabitur ligula sapien", 16)); // "Curabitur ligula..."
// console.log(formatMessage("Curabitur ligula sapien", 23)); // "Curabitur ligula sapien"
// console.log(formatMessage("Vestibulum facilisis purus nec", 20)); // "Vestibulum facilisis..."
// console.log(formatMessage("Vestibulum facilisis purus nec", 30)); // "Vestibulum facilisis purus nec"
// console.log(formatMessage("Nunc sed turpis a felis in nunc fringilla", 15)); // "Nunc sed turpis..."
// console.log(formatMessage("Nunc sed turpis a felis in nunc fringilla", 41)); // "Nunc sed turpis a felis in nunc fringilla"

3 Завдання:
//Друге рішення
// function checkForSpam(message) {
//     let lowerMessage = message.toLowerCase();
//     switch (true) {
//         case lowerMessage.includes('spam'):
//         case lowerMessage.includes('sale'):
//             return true;
//         default:
//             return false;
//     }
// }
// console.log(checkForSpam("Latest technology news")); // false
// console.log(checkForSpam("JavaScript weekly newsletter")); // false
// console.log(checkForSpam("Get best sale offers now!")); // true
// console.log(checkForSpam("Amazing SalE, only tonight!")); // true
// console.log(checkForSpam("Trust me, this is not a spam message")); // true
// console.log(checkForSpam("Get rid of sPaM emails. Our book in on sale!")); // true
// console.log(checkForSpam("[SPAM] How to earn fast money?")); // true


//Третє рішення
// function checkForSpam(message) {
//     let lowerMessage = (message.toLowerCase().includes('spam') || message.toLowerCase().includes('sale')) ? true : false;
//     return lowerMessage;
// }
// console.log(checkForSpam("Latest technology news")); // false
// console.log(checkForSpam("JavaScript weekly newsletter")); // false
// console.log(checkForSpam("Get best sale offers now!")); // true
// console.log(checkForSpam("Amazing SalE, only tonight!")); // true
// console.log(checkForSpam("Trust me, this is not a spam message")); // true
// console.log(checkForSpam("Get rid of sPaM emails. Our book in on sale!")); // true
// console.log(checkForSpam("[SPAM] How to earn fast money?")); // true

4 завдання:
//Друге рішення
// function getShippingCost(country) {
//     let price;
    
//     switch (country) {
//         case "China":
//             price = 100;
//             break;
//         case "Chile":
//             price = 250;
//             break;
//         case "Australia":
//             price = 170;
//             break;
//         case "Jamaica":
//             price = 120;
//             break;
//         default:
//             return "Sorry, there is no delivery to your country";
//     }
    
//     return `Shipping to ${country} will cost ${price} credits`;
// }

// console.log(getShippingCost("Australia")); // "Shipping to Australia will cost 170 credits"
// console.log(getShippingCost("Germany")); // "Sorry, there is no delivery to your country"
// console.log(getShippingCost("China")); // "Shipping to China will cost 100 credits"
// console.log(getShippingCost("Chile")); // "Shipping to Chile will cost 250 credits"
// console.log(getShippingCost("Jamaica")); // "Shipping to Jamaica will cost 120 credits"
// console.log(getShippingCost("Sweden")); // "Sorry, there is no delivery to your country"