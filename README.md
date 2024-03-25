class TravelPlanner:
    def __init__(self):
        self.budget = 0
        self.num_travelers = 0
        self.food_preferences = []
        self.places_to_visit = []
        self.travel_dates = {}
        self.destinations = []

    def set_budget(self, budget):
        self.budget = budget

    def set_num_travelers(self, num_travelers):
        self.num_travelers = num_travelers

    def set_food_preferences(self, food_preferences):
        self.food_preferences = food_preferences

    def set_places_to_visit(self, places_to_visit):
        self.places_to_visit = places_to_visit

    def set_travel_dates(self, travel_dates):
        self.travel_dates = travel_dates

    def set_destinations(self, destinations):
        self.destinations = destinations

    def generate_itinerary(self):
        # Placeholder function for generating itinerary based on preferences
        itinerary = {
            "Budget": self.budget,
            "Number of Travelers": self.num_travelers,
            "Food Preferences": self.food_preferences,
            "Places to Visit": self.places_to_visit,
            "Travel Dates": self.travel_dates,
            "Destinations": self.destinations
        }
        return itinerary


# Example usage
planner = TravelPlanner()

# Set traveler preferences
planner.set_budget(10000)
planner.set_num_travelers(2)
planner.set_food_preferences(["biryani", "dosa"])
planner.set_places_to_visit(["Museum", "Beach", "Park"])
planner.set_travel_dates({"start_date": "2024-06-01", "end_date": "2024-06-10"})
planner.set_destinations(["vizag", "araku"])

# Generate itinerary
itinerary = planner.generate_itinerary()

# Display itinerary
print("Generated Itinerary:")
for key, value in itinerary.items():
    print(key + ":", value)
