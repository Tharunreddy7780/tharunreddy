import datetime
import random

class TravelPlanner:
    def __init__(self, destination, budget, start_date, end_date):
        self.destination = destination
        self.budget = budget
        self.start_date = start_date
        self.end_date = end_date

    def generate_itinerary(self):
        # Sample implementation - replace with actual AI-based itinerary generation
        itinerary = {
            "Destination": self.destination,
            "Start Date": self.start_date,
            "End Date": self.end_date,
            "Activities": [
                "Rushikonda Beach",
                "Araku Valley",
                "Lighthouse"
            ],
            "Accommodation": "Hotel Novotel",
            "Transportation": "Flight IndiGo Airlines",
            "Total Cost": random.randint(self.budget // 2, self.budget)
        }
        return itinerary

# Example usage
destination = "vizag"
budget = 8000
start_date = datetime.date(2024, 4, 27)
end_date = datetime.date(2024, 5, 6)

planner = TravelPlanner(destination, budget, start_date, end_date)
itinerary = planner.generate_itinerary()
print("Generated Itinerary:")
print(itinerary)
