class Leavenfrosty {
  constructor(...options) {
    this.height = "1.80"
    this.weight = "90"
    this.type = "human"
    this.job = "Technical office engineer"
    this.gender = "male"
  }
}

class CreateMan extends Leavenfrosty {
  constructor(...options) {
    super(options);
  }

  private _eating() {
    void "eating 🍔 🍟 🍗 🥤"
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

let Leavenfrosty = new CreateMan()
Leavenfrosty.createDay();
<!---
leavenfrosty/leavenfrosty is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
