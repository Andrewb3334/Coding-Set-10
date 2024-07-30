# Coding-Set-10
Exercise 3

class Person:
    def __init__(self, name, address, age, phone_number):
        self._name = name
        self._address = address
        self._age = age
        self._phone_number = phone_number
    
    # Accessor methods
    def get_name(self):
        return self._name
    
    def get_address(self):
        return self._address
    
    def get_age(self):
        return self._age
    
    def get_phone_number(self):
        return self._phone_number
    
    # Mutator methods
    def set_name(self, name):
        self._name = name
    
    def set_address(self, address):
        self._address = address
    
    def set_age(self, age):
        self._age = age

    def set_phone_number(self, phone_number):
        self._phone_number = phone_number
    
    def __str__(self):
        return (f"Name {self._name}\n"
                f"Address: {self._address}\n"
                f"Age: {self._age}\n"
                f"Phone Number: {self._phone_number}")

#Example
def main():
    # Create an example using fictional information
    person1 = Person("James Williams", "564 Red Street, Orton", 35, "455-123-0074")
    person2 = Person("John Lewis", "466 Tree Road, Bridgington", 47, "910-093-2245")
    person3 = Person("Ron Deer", "590 Kensington Street, Bloomdale", 22, "810-969-7118")
    
    # Display information for the 3 people
    print("Person 1 Information:")
    print(person1)
    print("\nPerson 2 Information:")
    print(person2)
    print("\nPerson 3 Information:")
    print(person3)

if __name__ == "__main__":
      main()


Exercise 1

class Pet:
    def __init__(self, name= " " ,animal_type= " ", age=0)
        self._name = name
        self._animal_type = animal_type
        self._age = age

    # Mutator method
    def set_name(self, name):
        self._name = name

    def set_animal_type(self, animal_type):
        self._animal_type = animal_type

    def set_age(self, age):
        self._age = age

    # Accesor methods
    def get_name(self):
        return self._name

    def get_animal_type(self):
        return self._animal_type

    def get_age(self):
        return self._age
    
# Main program
def main():
    # Create a Pet object
    pet = Pet()

    # Prompt user for pet information
    name = input("Enter the name of your pet: ")
    animal_type = input("Enter the type of animal: ")
    age = int(input("Enter the age of your pet: "))

    # Set the attributes using setter methods
    pet.set_name(name)
    pet.set_animal_type(animal_type)
    pet.set_age(age)

    # Display pet information using getter methods
    print("\nPet Information: ")
    print(f"Name: {pet.get_name()}")
    print(f"Type: {pet.get_animal_type()}")
    print(f"Age: {pet.get_age()}")

if __name__ == "__main__"
    main()

