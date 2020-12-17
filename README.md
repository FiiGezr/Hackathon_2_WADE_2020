# WADe 2020 Hackhaton 2

# Proposal
Proposal
For week #11’s WADe lab (17 December, 12:00–16:00), the following challenge is proposed:
Sketch a 🦉conceptual model helping 🎅 to choose the right 🎁 – i.e. 🍭🦄🔬🎷⏳🚀💰 – to be placed under 🎄 by considering kids’ interests/hobbies (🎈🎶💻🍕📚👟) and their demographic profiles – 🗺️🏆👓🔞 –, plus weather/road conditions ⛅❄️🚧🚦.
[1 point bonus💎] Take into account the actual 🦠-related regulations.

# Our solution
### Classes and subclasses
* Person - https://www.wikidata.org/wiki/Q215627. We use this class as the parent class of the Child.
  * Child - https://www.wikidata.org/wiki/Q7569. Children are the most important part of this conceptual model because they are the ones receiving gifts from Santa.
* Hobby - https://www.wikidata.org/wiki/Q47728. A hobby is important because it can indicate what type of gift would be suitable for a child. Below we have some subclasses of hobbies to better indicate this.
  * Observation Hobby
  * Competitive Hobby
  * Educational Hobby
  * General Hobby
* Domain - A certain domain of interest.
* Gift - https://www.wikidata.org/wiki/Q184303. The class representing the gifts that Santa will deliver.
  * Product - https://www.wikidata.org/wiki/Q2424752. Subclass of gift, representing a material gift.
  * Experience - https://www.wikidata.org/wiki/Q18407687. Subclass of gift, representing a non-material gift.
* Location - https://www.wikidata.org/wiki/Q2221906. Geographic location.
* Characteristic - https://www.wikidata.org/wiki/Q1207505. We use this class to represent some demographic characteristics of the child, which again can influence the choice of a gift.
   * Social class - https://www.wikidata.org/wiki/Q187588
   * Nationality - https://www.wikidata.org/wiki/Q231002
   * Gender - https://www.wikidata.org/wiki/Q48277
   * Age - https://www.wikidata.org/wiki/Q185836
   * Education level - https://www.wikidata.org/wiki/Q18189
   * Disability - https://www.wikidata.org/wiki/Q12131
* Warning - https://www.wikidata.org/wiki/Q1759104. We use this class to indicate certain warnings related to a location.
   * Health Warning - Subclass of Warning.
      * Covid Warning - Subclass of Health Warning. Used to indicate the measures taken by the government at that location (e.g. quarantine, curfew, mask wearing)
### Relations
* subclassOf - Indicates that a class is a subclass of other, can be defined between any two classes.
* hasHobby - Domain: Person. Range: Hobby.  Indicates that a person has a certain hobby.
* isInterestedIn - Domain: Person. Range: Domain. Indicates that a person is interested in a certain domain of interest. (e.g. archery)
* livesAt - Domain: Person. Range: Location. Indicates that the person lives at a certain geographical location.
* hasCharacteristic - Domain: Person. Range: Characteristic. Indicates that a person has a demographic characteristic in our conceptual model.
* isRelatedTo - Domain: Gift. Range: Domain. Indicates that a gift is related to a certain domain of interest.(e.g. a bow is related to archery)
* foundAt - Domain: Product. Range: Location. Indicates that a product can be bought/order from a geographical location.
* takesPlaceAt - Domain: Experience. Range: Location. Indicates that an experience is happening at a geographical location. (e.g. Horse riding at the horse paddock)
* hasWarning - Domain: Location. Range: Warning. Indicates that there are certain warnings/measures of safety taken at a geographical location.
# Involvement of team members
* Baisan Razvan
  * visual representation of the conceptual model
  * A-box
* Florean Oana-Lavinia
  * visual representation of the conceptual model
  * A-box
* Gafitescu Petru-Marian
  * visual representation of the conceptual model
  * writing this document
