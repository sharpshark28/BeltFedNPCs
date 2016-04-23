# Belt Fed NPCs

##### Used to quickly generate NPCs with backgrounds and quirks.

### 😈 [See it in action](http://paulvmoreau.github.io/BeltFedNPCs/)

---

## About

NPCs are given reasonably weighted random races and other background details.

Names are created from a random first name and combined surnames to create a unique last name.

## Planned Improvements
 
I plan on adding more quirks and maneurisms as I go, but if you have any ideas then that would be great as well.

I also plan on developing a precompiler that would allow for each background to exist as it's own json file that get collected together into a single file at compile.

## Help the Project Grow

### Names

_(data/names.json)_

Feel free to add additional names, respecting gender neutrality produces the best results.

### Backgrounds

_(data/backgrounds.json)_

Example background layout:

```json
{
      "title": "Background Title",
      "description": "The introductory paragraph on the background. You can insert variable extras here by inserting <exampletag> and then including exampletag choices in the extras section. <otherexample>",
      "skillProficiencies": [
        "for now, this is text only"
      ],
      "Tool Proficiencies": ["Again, this will simply output whatever text is here"],
      "languages": [
        "this will output the text"
      ],
      "extras": [
        {
          "description": {
            "exampletag":[
              "Place a list here of random items you want to insert into <exampletag>.",
              "Because the parent of this object is named description, the program will find/replace for <exampletag> in description only.",
              "For now, the program does not do weighted random on these items",
              "Make sure your description has the right spacing before and after <exampletag> or it will look weird."
            ],
            "otherexample":[
              "keep in mind that the tags are case sensitive",
              "but you should be able to write any text for your tags as they will be replaced prior to being put on the page",
              "make sure you use unique tags or I cannot guarantee expected behavior"
            ]
          }
        }
      ],
      "equipment": "text only for now",
      "feature": "text only for now",
      "personalityTrait": [
        "Place any number of possible traits here",
        "One will be selected at random",
        "be creative, but the program will only pick one"
      ],
      "ideal": [
        "Place any number of possible ideals here",
        "One will be selected at random",
        "be creative, but the program will only pick one",
        "be sure to include alignment as needed",
      ],
      "bond": [
        "Place any number of possible traits here",
        "One will be selected at random",
        "be creative, but the program will only pick one"
      ],
      "flaw": [
        "Place any number of possible traits here",
        "One will be selected at random",
        "be creative, but the program will only pick one"
      ],
      "credit": "If you did not write this background. Please credit the creator here. Also, please avoid using lisenced backgrounds that you do not have rights to publish. you can also credit yourself here if you did create this background."
    }
```
