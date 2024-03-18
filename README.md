class Probabilities:
    def __init__(self):
        self.alias = ['diortemred', 'Whosdior']

    def contact(self):
        discord = 'diortemred'
        telegram = 'ttps://t.me/TokensSupplies'
        email = 'diorhosting@gmail.com'

        return discord, telegram, email

    def life(self):
        age = 15
        occupation = 'Student (Studying Computing & Networking)'
        hobbies = ['Programming', 'Reading']

        return age, occupation, hobbies

    def programming(self):
        languages = ['(Golang)', 'Python']
        learning = ['C# CPP']
        ide = 'Visual Studio Code'

        preferred_language = languages[0]

        return languages, learning, ide, preferred_language


if __name__ == "__main__":
    probabilities = Probabilities()
    discord, telegram, email = probabilities.contact()
    age, occupation, hobbies = probabilities.life()
    languages, learning, ide, preferred_language = probabilities.programming()

