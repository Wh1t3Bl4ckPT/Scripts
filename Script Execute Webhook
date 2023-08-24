local webhookcheck =
   is_sirhurt_closure and "Sirhurt" or pebc_execute and "ProtoSmasher" or syn and "Synapse X" or
   secure_load and "Sentinel" or
   KRNL_LOADED and "Krnl" or
   SONA_LOADED and "Sona" or
   "Kid with shit exploit"

local url =
   "https://discord.com/api/webhooks/1137823213292884048/XNWRhF_izBHfjfkbfInhL0pnpHSwwITyFjZuZoDl7ak7hGnUUEWTO-sImNy-He0CJhOq"
local data = {
   ["content"] = "||@everyone|| Script executed on https://roblox.com/games/" ..game.PlaceId.."",
   ["embeds"] = {
       {
           ["title"] = "**Someone Executed Your Script!**",
           ["description"] = "" .. game.Players.LocalPlayer.Name.." executed you'r script on https://roblox.com/games/".. game.PlaceId ..  " with **"..webhookcheck.."**",
           ["type"] = "rich",
           ["color"] = tonumber(0x7269da)
       }
   }
}
local newdata = game:GetService("HttpService"):JSONEncode(data)

local headers = {
   ["content-type"] = "application/json"
}
request = http_request or request or HttpPost or syn.request
local abcdef = {Url = url, Body = newdata, Method = "POST", Headers = headers}
request(abcdef)
