javascript:(function() {

const key = {
sound:0.7,
music:0.3,
score:0,
hasShownTutorial:true,
collectedCoin:0,
cars:[0],
currentCar:0,
currentTip:0,
booster1:1,
booster2:1,
booster3:1,
ko:0,
hasShownBoosterTutorial:true
};

localStorage.setItem(
"mjs-drift-boss-game-v1.0.1-dailyreward",
JSON.stringify(key)
);

window.location.reload();

})();