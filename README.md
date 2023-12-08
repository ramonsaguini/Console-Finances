
//! ////////////////// Total Months
console.log("Total Months: " + finances.length);


//? //////////////// Total value
var sum = 0;

for (var i = 0; i < finances.length; i++) {
  sum += finances[i][1];
}
console.log("Total: $" + sum);


//* /////////// Average calc
console.log("Average Change: $" + (sum / finances.length - 1).toFixed(2));


////////////////! Greatest value
finances.sort((a, b) => b[1] - a[1]);

console.log(`Greatest Increase in Profits/Losses: ${finances[0][0]} ($${finances[0][1]})`);


// console.log("Greateste Decrease in Profits/Losses: " + );

finances.sort((a, b) => a[1] - b[1]);

console.log(`Greatest Decrease in Profits/Losses: ${finances[0][0]} ($${finances[0][1]})`);
