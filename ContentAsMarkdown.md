harrastuksia = true
if harrastus == true then
	print("Minulla on harrastuksia")
else
	print("Ei ole harrastuksia")
end


harrastus = script.Parent.StringValue.Value
if harrastus == "Legojen keräily" then
      print ("Legojen keräily")
end
function Ulkoilu()
	if game.Universe.Maapallo.Weather.Value == "Sunny" then
          print("Menen ulos ja otan valokuvia")
        else
          print("Olen sisällä ja olen tietokoneella tai rakentelen.")
		end
end

script.Parent.Parent.Players.Robban.Thoughts.Changed:Connect(Ulkoilu)
