
class Weather:
    def __init__(self, parameters):
        self.parameters = parameters

    def __contains__(self, item):
        return item in self.parameters

    def __str__(self):
        return f"Weather Parameters: {', '.join(self.parameters)}"

today_weather = Weather(["Sunny", "Windy", "Dry"])

print(today_weather)

print("\nIs it Sunny today?", "Sunny" in today_weather)
print("Is it Rainy today?", "Rainy" in today_weather)
