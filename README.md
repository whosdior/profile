class ClutchBets:
    def __init__(self):
        self.company = {
            "name": "ClutchBets",
            "website": "https://clutchbets.online/",
            "support_email": "support@clutchbets.online"
        }

        self.leadership = {
            "CEO": {
                "name": "whodior",
                "aliases": ["diortemred", "Whosdior"],
                "discord": "main.go."
            }
        }

        self.contact = {
            "Main Discord": "diorsfakealt",
            "CEO Discord": self.leadership["CEO"]["discord"],
            "Support Email": self.company["support_email"]
        }

        self.platform = {
            "type": "Betting / Picks Platform",
            "focus": ["Outlier Bets", "Analytics", "User Picks"],
            "status": "Active"
        }

        self.features = [
            "User pick tracking",
            "Performance analytics",
            "Optimized dashboard",
            "Mobile + desktop support"
        ]

    def summary(self):
        return {
            "Company": self.company["name"],
            "Website": self.company["website"],
            "CEO": self.leadership["CEO"]["name"]
        }

    def display(self):
        print("=" * 50)
        print("CLUTCHBETS OVERVIEW")
        print("=" * 50)

        print("\nCompany:")
        for k, v in self.company.items():
            print(f" {k}: {v}")

        print("\nLeadership:")
        ceo = self.leadership["CEO"]
        print(f" Name: {ceo['name']}")
        print(f" Aliases: {', '.join(ceo['aliases'])}")
        print(f" Discord: {ceo['discord']}")

        print("\nContact:")
        for k, v in self.contact.items():
            print(f" {k}: {v}")

        print("\nPlatform:")
        for k, v in self.platform.items():
            print(f" {k}: {v}")

        print("\nFeatures:")
        for f in self.features:
            print(f" - {f}")

        print("=" * 50)


if __name__ == "__main__":
    clutch = ClutchBets()
    clutch.display()
