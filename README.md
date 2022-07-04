<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Thanks again! Now go create something AMAZING! :D
-->

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->

[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
    <img src="resources/icon.png" alt="Logo" width="80" height="80">

  <h3 align="center">SnackScan - Official repository</h3>

  <p>
    Welcome to the official repository of the most complete purchase management application in the market. In this repository you can collaborate with the project by helping us to complete translations or information about additives. <br/> <br/>You can also ask questions, make suggestions, report errors... For all that, check the following <a href="https://github.com/enriqueloz88/SnackScan/issues">link</a>. There you will see a list of suggestions for improvement, as well as known bugs. You can add new issues, as long as no other user has already posted the same issue.
  </p>
</p>

[<img src="https://play.google.com/intl/en_us/badges/images/generic/en-play-badge.png"
     alt="Get it on Google Play"
     height="80">](https://play.google.com/store/apps/details?id=com.snackscan.app)

<!-- CONTRIBUTING -->

## Contributing 🙋🏻

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Translation

The translations are in a json format <a href="https://github.com/enriqueloz88/SnackScan/tree/main/i18n">here</a>. To generate a new language you only have to create a new file _lang.json_ where you must replace "lang" by the code of the language in question. You can extract these codes from this <a href="https://www.loc.gov/standards/iso639-2/php/code_list.php">link</a> looking at the ISO 639-1 Code column.

It is important that all new json files generated have exactly the same keys as the files already exposed. It is recommended to look at the _en.json_ file for reference. You can also modify any existing translation file, if you consider that any translation can be improved.

### Additives

Help with the additives information is very easy. You just need to open the file _additives.ts_ of this project and do the changes that you consider necesary. Please, bear in mind that if you copy some literal content from internet you must add the source in the sources array. An example of an additive object is shown bellow:

```
  {
    "code": "E102",
    "description": {
      "es": "text-in-spanish....",
      "en": "This compound dissolves in water, turning more yellow as its amount increases in solution. It is commonly used in desserts, gum, gummies, energy drinks and snacks. <br> Many colorants of this family (not those authorized for food use) have been shown to be carcinogenic, although there is no evidence of this being so. However, there is evidence that this compound mixed with other additives can cause hyperactivity in minors"
    },
    "name": {
      "en": "Tartrazine",
      "es": "Tartrazina"
    },
    "toxicity": "High",
    "sources": [
      "McCann y col. (2007) 'Food additives and hyperactive behaviour in 3-year-old and 8/9-year-old children in the community: a randomised, double-blinded, placebo-controlled trial.' Lancet. 370(9598):1560-7."
    ]
  },
```

To add a new paragraph in the additive description, don't use \n or similar, use the `<br>` tag. If you add new languages in the previous section, you can also do it here, both for the _name_ and _description_ attributes. Remember that these new languages will always be optional attributes, the only mandatory language is English.

<!-- CONTACT -->

## Contact 📧

Enrique Lozano - kikelozano8@gmail.com

Project Link: [https://github.com/enriqueloz88/SnackScan](https://github.com/enriqueloz88/SnackScan)

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/enrique-lozano-cebriano/
