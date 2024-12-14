# LA-16

class Appliance():
    def __init__(self, brand, model, info):
        self.brand = brand
        self.model = model
        self.info = info
        
    def operate(self):
        print("Operating")
        
class WashingMachine(Appliance):
    def __init__(self, brand, model, info):
        super().__init__(brand, model, info)
        
    def operate(self):
        print("Washing clothes!")
        
class Refrigerator(Appliance):
    def __init__(self, brand, model, info):
        super().__init__(brand, model, info)
        
    def operate(self):
        print("Keeping food cold!")
        
class Microwave(Appliance):
    def __init__(self, brand, model, info):
        super().__init__(brand, model, info)
        
    def operate(self):
        print("Heating food!")

wash = WashingMachine("Samsung", "WD16T6300GP Washer/Dryer", "quality")
ref = Refrigerator("Samsung", "SBS Family Hub", "qualty")
micro = Microwave("Samsung", "TC", "quality")

for appliance in [wash, ref, micro]:
    appliance.operate()
