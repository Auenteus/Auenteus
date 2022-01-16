class Auenteus {
  constructor(...options) {
    this.height = "1.77"
    this.weight = "66"
    this.type = "human"
    this.job = "student"
    this.sex = "male"
  }
}

class CreateMan extends Auenteus {
  constructor(...options) {
    super(options);
  }
  
  private _eating() {
    void "eating 🍔 🍟 🥤"
  }
  
  private _coding() {
    void "coding... ❤️"
  }
  
  private _sleep(ms) { return new Promise(resolve => setTimeout(resolve, ms)) }
  
  async createDay() {
    this._eating()
    this._coding()
    await this._sleep(18000000)
    
    this.createDay()
  }
       
} 

let Auenteus = new CreateMan()
auenteus.createDay();
