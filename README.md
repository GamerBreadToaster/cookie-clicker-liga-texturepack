# cookie-clicker-liga-texturepack
a tempermonkey script

copy this under here:

// ==UserScript==
// @name         cookie clicker liga texture pack
// @namespace    http://tampermonkey.net/
// @version      0.1
// @description  try to take over the world!
// @author       GamerBreadToaster
// @match        http://orteil.dashnet.org/cookieclicker/
// @icon         https://www.google.com/s2/favicons?domain=dashnet.org
// @grant        none
// ==/UserScript==

(function() {
    'use strict';

    const waitIntervalId = setInterval(function() {
        if (typeof Game !== 'undefined') {
            clearInterval(waitIntervalId);
            loadPictures();
        }
    }, 1000);


    function loadPictures(){
        Game.Loader.Replace("perfectCookie.png", "https://www.liga.nl/wp-content/uploads/2021/01/LIGA_Milkbreak_Melk_.png")
        Game.Loader.Replace("smallCookies.png", "https://www.liga.nl/wp-content/uploads/2021/01/LIGA_Milkbreak_Melk_.png")
        Game.Loader.Replace("imperfectCookie.png", "https://www.liga.nl/wp-content/uploads/2021/01/LIGA_Milkbreak_Melk_.png")
        Game.Loader.Replace("icons.png", "https://i.redd.it/6e3vagip4gsa1.png")
    };
})();
