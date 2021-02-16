# GPT2 Game Of Thrones

[![Run on Ainize](https://ainize.ai/images/run_on_ainize_button.svg)](https://ainize.web.app/redirect?git_repo=https://github.com/fpem123/GPT2-GameOfThrones)

This project generate Game Of Thrones script using GPT-2 model.

Fine tuning data: [Kaggle](https://www.kaggle.com/albenft/game-of-thrones-script-all-seasons)

### Model information

    Base model: gpt-2 large
    Epoch: 30
    Train runtime: 3060.6076 secs
    Loss: 0.0232

### How to use

    * First, Choose Game Of Thrones character name.
    * Second, Fill what the character will say in text. This will be base of script.
    * And then, Fill number in length. Text is created as long as "length". I recommend between 100 and 300.
    * If length is so big, generate time will be long.

### Post parameter

    name: The Game Of Thrones character name.
    text: The base of script.
    length: The size of generated text.(min: 50)

### Output foramt

    {"0": [[character name, dialog], [character name, dialog], ...]}


### Image reference

[static/README.md]()

## * With CLI *

#### Input example

    curl -X POST "https://master-gpt2-game-of-thrones-fpem123.endpoint.ainize.ai/gameofthrones" -H "accept: application/json" -H "Content-Type: multipart/form-data" -F "name=jon snow" -F "text=Hello" -F "length=150"

#### Output example




## * With swagger *

API page: [Ainize](https://ainize.ai/fpem123/GPT2-GameOfThrones?branch=master)

## * With a Demo *

Demo page: [End-point](https://master-gpt2-game-of-thrones-fpem123.endpoint.ainize.ai/)