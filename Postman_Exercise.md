GET www.thecocktaildb.com/api/json/v1/1/search.php?s=margarita

{
    "drinks": [
        {
            "idDrink": "11007",
            "strDrink": "Margarita",
            "strDrinkAlternate": null,
            "strTags": "IBA,ContemporaryClassic",
            "strVideo": null,
            "strCategory": "Ordinary Drink",
            "strIBA": "Contemporary Classics",
            "strAlcoholic": "Alcoholic",
            "strGlass": "Cocktail glass",
            "strInstructions": "Rub the rim of the glass with the lime slice to make the salt stick to it. Take care to moisten only the outer rim and sprinkle the salt on it. The salt should present to the lips of the imbiber and never mix into the cocktail. Shake the other ingredients with ice, then carefully pour into the glass.",
            "strInstructionsES": null,
            "strInstructionsDE": "Reiben Sie den Rand des Glases mit der Limettenscheibe, damit das Salz daran haftet. Achten Sie darauf, dass nur der äußere Rand angefeuchtet wird und streuen Sie das Salz darauf. Das Salz sollte sich auf den Lippen des Genießers befinden und niemals in den Cocktail einmischen. Die anderen Zutaten mit Eis schütteln und vorsichtig in das Glas geben.",
            "strInstructionsFR": null,
            "strInstructionsIT": "Strofina il bordo del bicchiere con la fetta di lime per far aderire il sale.\r\nAvere cura di inumidire solo il bordo esterno e cospargere di sale.\r\nIl sale dovrebbe presentarsi alle labbra del bevitore e non mescolarsi mai al cocktail.\r\nShakerare gli altri ingredienti con ghiaccio, quindi versarli delicatamente nel bicchiere.",
            "strInstructionsZH-HANS": null,
            
          .....
}

--------------------------------------------------------------------------------------------------------------------------------------------------

GET www.thecocktaildb.com/api/json/v1/1/search.php?i=vodka
{
    "ingredients": [
        {
            "idIngredient": "1",
            "strIngredient": "Vodka",
            "strDescription": "Vodka is a distilled beverage composed primarily of water and ethanol, sometimes with traces of impurities and flavorings. Traditionally, vodka is made by the distillation of fermented cereal grains or potatoes, though some modern brands use other substances, such as fruits or sugar.\r\n\r\nSince the 1890s, the standard Polish, Russian, Belarusian, Ukrainian, Estonian, Latvian, Lithuanian and Czech vodkas are 40% alcohol by volume ABV (80 US proof), a percentage that is widely misattributed to Dmitri Mendeleev. The European Union has established a minimum of 37.5% ABV for any \"European vodka\" to be named as such. Products sold as \"vodka\" in the United States must have a minimum alcohol content of 40%. Even with these loose restrictions, most vodka sold contains 40% ABV. For homemade vodkas and distilled beverages referred to as \"moonshine\", see moonshine by country.\r\n\r\nVodka is traditionally drunk neat (not mixed with any water, ice, or other mixer), though it is often served chilled in the vodka belt countries (Belarus, Estonia, Finland, Iceland, Latvia, Lithuania, Norway, Poland, Russia, Sweden, Ukraine). It is also commonly used in cocktails and mixed drinks, such as the vodka martini, Cosmopolitan, vodka tonic, Screwdriver, Greyhound, Black or White Russian, Moscow Mule, and Bloody Mary.\r\n\r\nScholars debate the beginnings of vodka. It is a contentious issue because very little historical material is available. For many centuries, beverages differed significantly compared to the vodka of today, as the spirit at that time had a different flavor, color and smell, and was originally used as medicine. It contained little alcohol, an estimated maximum of about 14%, as only this amount can be attained by natural fermentation. The still, allowing for distillation (\"burning of wine\"), increased purity, and increased alcohol content, was invented in the 8th century.\r\n\r\nA common property of the vodkas produced in the United States and Europe is the extensive use of filtration prior to any additional processing including the addition of flavorants. Filtering is sometimes done in the still during distillation, as well as afterwards, where the distilled vodka is filtered through activated charcoal and other media to absorb trace amounts of substances that alter or impart off-flavors to the vodka. However, this is not the case in the traditional vodka-producing nations, so many distillers from these countries prefer to use very accurate distillation but minimal filtering, thus preserving the unique flavors and characteristics of their products.\r\n\r\nThe master distiller is in charge of distilling the vodka and directing its filtration, which includes the removal of the \"fore-shots\", \"heads\" and \"tails\". These components of the distillate contain flavor compounds such as ethyl acetate and ethyl lactate (heads) as well as the fusel oils (tails) that impact the usually desired clean taste of vodka. Through numerous rounds of distillation, or the use of a fractioning still, the taste is modified and clarity is increased. In contrast, distillery process for liquors such as whiskey, rum, and baijiu allow portions of the \"heads\" and \"tails\" to remain, giving them their unique flavors.\r\n\r\nRepeated distillation of vodka will make its ethanol level much higher than is acceptable to most end users, whether legislation determines strength limits or not. Depending on the distillation method and the technique of the stillmaster, the final filtered and distilled vodka may have as much as 95–96% ethanol. As such, most vodka is diluted with water prior to bottling.\r\n\r\nPolish distilleries make a very pure (96%, 192 proof, formerly also 98%) rectified spirit (Polish language: spirytus rektyfikowany). Technically a form of vodka, it is sold in liquor stores rather than pharmacies. Similarly, the German market often carries German, Hungarian, Polish, and Ukrainian-made varieties of vodka of 90 to 95% ABV. A Bulgarian vodka, Balkan 176°, has an 88% alcohol content. Everclear, an American brand, is also sold at 95% ABV.",
            "strType": "Vodka",
            "strAlcohol": "Yes",
            "strABV": "40"
        }
    ]
}
--------------------------------------------------------------------------------------------------------------------------------------------------------

GET https://dummy.restapiexample.com/api/v1/employee/14

{
    "status": "success",
    "data": {
        "id": 14,
        "employee_name": "Haley Kennedy",
        "employee_salary": 313500,
        "employee_age": 43,
        "profile_image": ""
    },
    "message": "Successfully! Record has been fetched."
}
-----------------------------------------------------------------------------------------------------------------------------------------------------------

PUT https://dummy.restapiexample.com/api/v1/update/14
body raw json {
  "name": "John",
  "salary": "40000",
  "age": "35"
}

{
    "status": "success",
    "data": {
        "name": "John",
        "salary": "40000",
        "age": "35"
    },
    "message": "Successfully! Record has been updated."
}
--------------------------------------------------------------------------------------------------------------------------------------------------------------

GET https://api.agify.io?name[]=lucy&name[]=bob&name[]=alice

[
    {
        "age": 56,
        "count": 25515,
        "name": "lucy"
    },
    {
        "age": 69,
        "count": 43997,
        "name": "bob"
    },
    {
        "age": 55,
        "count": 69230,
        "name": "alice"
    }
]
