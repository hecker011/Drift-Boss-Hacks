javascript:(function() {
const coins = Number(prompt("How Many Coins Do You Want?", "1"));
const s = Number(prompt("How much score do you want?", "1"));
const doubleScore = Number(prompt("How much double score powerups do you want?", "1"));
const insurance = Number(prompt("How much car insurance do you want?", "1"));
const coinBoost = Number(prompt("How much coin boost do you want?", "1"));
const carNumber = Number(prompt("Which car do you want (car number)", "0"));

let c = [];

for(let i = 0; i < 27; i++) {
 c.push(i);
};

const key = {
sound:0.7,
music:0.3,
score:s,
hasShownTutorial:true,
collectedCoin:coins,
cars:c,
currentCar:carNumber,
currentTip:0,
booster1:doubleScore,
booster2:insurance,
booster3:coinBoost,
ko:0,
hasShownBoosterTutorial:true
};

localStorage.setItem(
"mjs-drift-boss-game-v1.0.1-dailyreward",
JSON.stringify(key)
);

window.location.reload();

})();