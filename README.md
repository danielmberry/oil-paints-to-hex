# Finding the Hex and RGB values for Williamsburg Oil Paints

## Introduction
The idea for this project came from a conversation I had with a designer who wanted to get my input on colors to use for a user interface. While I was able to help to an extent, as a painter, my mind works more in oil paint colors than it does in hex or RGB colors. 

Following our conversation, I decided to create a script that would gather all of the oil paint swatch images from the website of my favorite oil paint company, [Williamsburg Oils](https://www.williamsburgoils.com), and process each image, finding the median hex and RGB values within the image using computer vision and KMeans clustering.

The end result is the table at the end of this README, where I've listed the hex color and corresponding RGB color next to the original image pulled from Williamsburg Oils' website. 

Please note that the resulting hex/RGB color resulting from the program is simply the median value derived from the KMeans clustering program with `n_clusters` set to `1`. Additionally, the resulting value is unlikely to be an exact match to the oil paint color due to the transparent/opaque properties of oil paints, and differences in how colors appear to the human eye in-person versus through a computer screen. 

## Method



## Color List
|Color Name|Hex color|RGB Color|Paint swatch|Returned color|
|-----|-----|-----|-----|-----|
|Alizarin Crimson|#92343f|[146, 52, 63]|![](./images/alizarin_crimson_swatch.jpg)|![](./returned_colors/alizarin_crimson_returned.jpg)|
|Alizarin Orange|#9f471b|[159, 71, 27]|![](./images/alizarin_orange_swatch.jpg)|![](./returned_colors/alizarin_orange_returned.jpg)|
|Alizarin Yellow|#c88c1b|[200, 140, 27]|![](./images/alizarin_yellow_swatch.jpg)|![](./returned_colors/alizarin_yellow_returned.jpg)|
|Bismuth Vanadate Yellow|#f6df08|[246, 223, 8]|![](./images/bismuth_vanadate_yellow_swatch.jpg)|![](./returned_colors/bismuth_vanadate_yellow_returned.jpg)|
|Bohemian Green Earth|#474b3b|[71, 75, 59]|![](./images/bohemian_green_earth_swatch.jpg)|![](./returned_colors/bohemian_green_earth_returned.jpg)|
|Brilliant Yellow Extra Pale|#f9f4d7|[249, 244, 215]|![](./images/brilliant_yellow_extra_pale_swatch.jpg)|![](./returned_colors/brilliant_yellow_extra_pale_returned.jpg)|
|Brilliant Yellow Pale|#f6eea7|[246, 238, 167]|![](./images/brilliant_yellow_pale_swatch.jpg)|![](./returned_colors/brilliant_yellow_pale_returned.jpg)|
|Brown Ochre|#78613f|[120, 97, 63]|![](./images/brown_ochre_swatch.jpg)|![](./returned_colors/brown_ochre_returned.jpg)|
|Brown Pink|#3c3632|[60, 54, 50]|![](./images/brown_pink_swatch.jpg)|![](./returned_colors/brown_pink_returned.jpg)|
|Brown Umber|#191610|[25, 22, 16]|![](./images/brown_umber_swatch.jpg)|![](./returned_colors/brown_umber_returned.jpg)|
|Burnt Sienna|#764b3d|[118, 75, 61]|![](./images/burnt_sienna_swatch.jpg)|![](./returned_colors/burnt_sienna_returned.jpg)|
|Burnt Umber|#2c2b24|[44, 43, 36]|![](./images/burnt_umber_swatch.jpg)|![](./returned_colors/burnt_umber_returned.jpg)|
|Cadmium Green|#45732d|[69, 115, 45]|![](./images/cadmium_green_swatch.jpg)|![](./returned_colors/cadmium_green_returned.jpg)|
|Cadmium Green Light|#6f9839|[111, 152, 57]|![](./images/cadmium_green_light_swatch.jpg)|![](./returned_colors/cadmium_green_light_returned.jpg)|
|Cadmium Lemon|#ece040|[236, 224, 64]|![](./images/cadmium_lemon_swatch.jpg)|![](./returned_colors/cadmium_lemon_returned.jpg)|
|Cadmium Orange|#f69821|[246, 152, 33]|![](./images/cadmium_orange_swatch.jpg)|![](./returned_colors/cadmium_orange_returned.jpg)|
|Cadmium Purple|#804b45|[128, 75, 69]|![](./images/cadmium_purple_swatch.jpg)|![](./returned_colors/cadmium_purple_returned.jpg)|
|Cadmium Red Deep|#802315|[128, 35, 21]|![](./images/cadmium_red_deep_swatch.jpg)|![](./returned_colors/cadmium_red_deep_returned.jpg)|
|Cadmium Red Light|#e55305|[229, 83, 5]|![](./images/cadmium_red_light_swatch.jpg)|![](./returned_colors/cadmium_red_light_returned.jpg)|
|Cadmium Red Medium|#a53019|[165, 48, 25]|![](./images/cadmium_red_medium_swatch.jpg)|![](./returned_colors/cadmium_red_medium_returned.jpg)|
|Cadmium Red Purple|#6e2f26|[110, 47, 38]|![](./images/cadmium_red_purple_swatch.jpg)|![](./returned_colors/cadmium_red_purple_returned.jpg)|
|Cadmium Red Vermillion|#dc5430|[220, 84, 48]|![](./images/cadmium_red_vermillion_swatch.jpg)|![](./returned_colors/cadmium_red_vermillion_returned.jpg)|
|Cadmium Yellow Deep|#edc02f|[237, 192, 47]|![](./images/cadmium_yellow_deep_swatch.jpg)|![](./returned_colors/cadmium_yellow_deep_returned.jpg)|
|Cadmium Yellow Extra Deep|#f49c0c|[244, 156, 12]|![](./images/cadmium_yellow_extra_deep_swatch.jpg)|![](./returned_colors/cadmium_yellow_extra_deep_returned.jpg)|
|Cadmium Yellow Light|#e9d61f|[233, 214, 31]|![](./images/cadmium_yellow_light_swatch.jpg)|![](./returned_colors/cadmium_yellow_light_returned.jpg)|
|Cadmium Yellow Medium|#f0d32b|[240, 211, 43]|![](./images/cadmium_yellow_medium_swatch.jpg)|![](./returned_colors/cadmium_yellow_medium_returned.jpg)|
|Canton Rose|#d0886b|[208, 136, 107]|![](./images/canton_rose_swatch.jpg)|![](./returned_colors/canton_rose_returned.jpg)|
|Carl's Crimson (Permanent)|#792b26|[121, 43, 38]|![](./images/carl's_crimson_(permanent)_swatch.jpg)|![](./returned_colors/carl's_crimson_(permanent)_returned.jpg)|
|Cerulean Blue (Genuine)|#154085|[21, 64, 133]|![](./images/cerulean_blue_(genuine)_swatch.jpg)|![](./returned_colors/cerulean_blue_(genuine)_returned.jpg)|
|Cerulean Blue French|#354a83|[53, 74, 131]|![](./images/cerulean_blue_french_swatch.jpg)|![](./returned_colors/cerulean_blue_french_returned.jpg)|
|Chromium Oxide Green|#446b2a|[68, 107, 42]|![](./images/chromium_oxide_green_swatch.jpg)|![](./returned_colors/chromium_oxide_green_returned.jpg)|
|Cinnabar Green Light|#b2b235|[178, 178, 53]|![](./images/cinnabar_green_light_swatch.jpg)|![](./returned_colors/cinnabar_green_light_returned.jpg)|
|Cobalt Blue|#2f3d8a|[47, 61, 138]|![](./images/cobalt_blue_swatch.jpg)|![](./returned_colors/cobalt_blue_returned.jpg)|
|Cobalt Blue Deep|#374eaa|[55, 78, 170]|![](./images/cobalt_blue_deep_swatch.jpg)|![](./returned_colors/cobalt_blue_deep_returned.jpg)|
|Cobalt Green|#1b581e|[27, 88, 30]|![](./images/cobalt_green_swatch.jpg)|![](./returned_colors/cobalt_green_returned.jpg)|
|Cobalt Teal Bluish|#0fa796|[15, 167, 150]|![](./images/cobalt_teal_bluish_swatch.jpg)|![](./returned_colors/cobalt_teal_bluish_returned.jpg)|
|Cobalt Teal Greenish|#4aa695|[74, 166, 149]|![](./images/cobalt_teal_greenish_swatch.jpg)|![](./returned_colors/cobalt_teal_greenish_returned.jpg)|
|Cobalt Turqoise Bluish|#1d3465|[29, 52, 101]|![](./images/cobalt_turqoise_bluish_swatch.jpg)|![](./returned_colors/cobalt_turqoise_bluish_returned.jpg)|
|Cobalt Turqoise Greenish|#17455d|[23, 69, 93]|![](./images/cobalt_turqoise_greenish_swatch.jpg)|![](./returned_colors/cobalt_turqoise_greenish_returned.jpg)|
|Cobalt Violet Deep|#1e0b43|[30, 11, 67]|![](./images/cobalt_violet_deep_swatch.jpg)|![](./returned_colors/cobalt_violet_deep_returned.jpg)|
|Cobalt Violet Light|#af6993|[175, 105, 147]|![](./images/cobalt_violet_light_swatch.jpg)|![](./returned_colors/cobalt_violet_light_returned.jpg)|
|Cobalt Yellow|#d9b32d|[217, 179, 45]|![](./images/cobalt_yellow_swatch.jpg)|![](./returned_colors/cobalt_yellow_returned.jpg)|
|Cold Black|#343c46|[52, 60, 70]|![](./images/cold_black_swatch.jpg)|![](./returned_colors/cold_black_returned.jpg)|
|Courbet Green|#0d1d10|[13, 29, 16]|![](./images/courbet_green_swatch.jpg)|![](./returned_colors/courbet_green_returned.jpg)|
|Cyprus Orange|#a05818|[160, 88, 24]|![](./images/cyprus_orange_swatch.jpg)|![](./returned_colors/cyprus_orange_returned.jpg)|
|Davy's Grey Deep|#373b38|[55, 59, 56]|![](./images/davy's_grey_deep_swatch.jpg)|![](./returned_colors/davy's_grey_deep_returned.jpg)|
|Dianthus Pink|#eba4af|[235, 164, 175]|![](./images/dianthus_pink_swatch.jpg)|![](./returned_colors/dianthus_pink_returned.jpg)|
|Dutch Brown (Transparent)|#1c1c1c|[28, 28, 28]|![](./images/dutch_brown_(transparent)_swatch.jpg)|![](./returned_colors/dutch_brown_(transparent)_returned.jpg)|
|Earth Green|#424a2c|[66, 74, 44]|![](./images/earth_green_swatch.jpg)|![](./returned_colors/earth_green_returned.jpg)|
|Egyptian Violet|#05070e|[5, 7, 14]|![](./images/egyptian_violet_swatch.jpg)|![](./returned_colors/egyptian_violet_returned.jpg)|
|Fanchon Red|#be381a|[190, 56, 26]|![](./images/fanchon_red_swatch.jpg)|![](./returned_colors/fanchon_red_returned.jpg)|
|Flake White|#fefbdd|[254, 251, 221]|![](./images/flake_white_swatch.jpg)|![](./returned_colors/flake_white_returned.jpg)|
|French Ardoise Gray|#aea498|[174, 164, 152]|![](./images/french_ardoise_gray_swatch.jpg)|![](./returned_colors/french_ardoise_gray_returned.jpg)|
|French Brown Ochre|#504032|[80, 64, 50]|![](./images/french_brown_ochre_swatch.jpg)|![](./returned_colors/french_brown_ochre_returned.jpg)|
|French Burnt Ochre|#36281c|[54, 40, 28]|![](./images/french_burnt_ochre_swatch.jpg)|![](./returned_colors/french_burnt_ochre_returned.jpg)|
|French Burnt Umber|#564c41|[86, 76, 65]|![](./images/french_burnt_umber_swatch.jpg)|![](./returned_colors/french_burnt_umber_returned.jpg)|
|French Light Sienna|#8c7b56|[140, 123, 86]|![](./images/french_light_sienna_swatch.jpg)|![](./returned_colors/french_light_sienna_returned.jpg)|
|French Ochre Havane|#c19167|[193, 145, 103]|![](./images/french_ochre_havane_swatch.jpg)|![](./returned_colors/french_ochre_havane_returned.jpg)|
|French Raw Sienna|#b4802e|[180, 128, 46]|![](./images/french_raw_sienna_swatch.jpg)|![](./returned_colors/french_raw_sienna_returned.jpg)|
|French Raw Umber|#8b8069|[139, 128, 105]|![](./images/french_raw_umber_swatch.jpg)|![](./returned_colors/french_raw_umber_returned.jpg)|
|French Rouge Indian|#8a5246|[138, 82, 70]|![](./images/french_rouge_indian_swatch.jpg)|![](./returned_colors/french_rouge_indian_returned.jpg)|
|French Terre Verte|#8ca59c|[140, 165, 156]|![](./images/french_terre_verte_swatch.jpg)|![](./returned_colors/french_terre_verte_returned.jpg)|
|French Yellow Ochre Deep|#b5853d|[181, 133, 61]|![](./images/french_yellow_ochre_deep_swatch.jpg)|![](./returned_colors/french_yellow_ochre_deep_returned.jpg)|
|German Earth|#1b201e|[27, 32, 30]|![](./images/german_earth_swatch.jpg)|![](./returned_colors/german_earth_returned.jpg)|
|Graphite Gray|#565752|[86, 87, 82]|![](./images/graphite_gray_swatch.jpg)|![](./returned_colors/graphite_gray_returned.jpg)|
|Green Gold|#17220c|[23, 34, 12]|![](./images/green_gold_swatch.jpg)|![](./returned_colors/green_gold_returned.jpg)|
|Indanthrone Blue|#141839|[20, 24, 57]|![](./images/indanthrone_blue_swatch.jpg)|![](./returned_colors/indanthrone_blue_returned.jpg)|
|Indian Yellow|#de8207|[222, 130, 7]|![](./images/indian_yellow_swatch.jpg)|![](./returned_colors/indian_yellow_returned.jpg)|
|Indigo|#1e2b31|[30, 43, 49]|![](./images/indigo_swatch.jpg)|![](./returned_colors/indigo_returned.jpg)|
|Interference Blue|#c1cad2|[193, 202, 210]|![](./images/interference_blue_swatch.jpg)|![](./returned_colors/interference_blue_returned.jpg)|
|Interference Green|#f1ecd8|[241, 236, 216]|![](./images/interference_green_swatch.jpg)|![](./returned_colors/interference_green_returned.jpg)|
|Interference Red|#e4d3b8|[228, 211, 184]|![](./images/interference_red_swatch.jpg)|![](./returned_colors/interference_red_returned.jpg)|
|Interference Violet|#dacbbd|[218, 203, 189]|![](./images/interference_violet_swatch.jpg)|![](./returned_colors/interference_violet_returned.jpg)|
|Iridescent Bronze|#7a6a54|[122, 106, 84]|![](./images/iridescent_bronze_swatch.jpg)|![](./returned_colors/iridescent_bronze_returned.jpg)|
|Iridescent Copper|#b36540|[179, 101, 64]|![](./images/iridescent_copper_swatch.jpg)|![](./returned_colors/iridescent_copper_returned.jpg)|
|Iridescent Pale Gold|#f3dca9|[243, 220, 169]|![](./images/iridescent_pale_gold_swatch.jpg)|![](./returned_colors/iridescent_pale_gold_returned.jpg)|
|Iridescent Pearl White|#d9d0ba|[217, 208, 186]|![](./images/iridescent_pearl_white_swatch.jpg)|![](./returned_colors/iridescent_pearl_white_returned.jpg)|
|Iridescent Pewter|#4f5153|[79, 81, 83]|![](./images/iridescent_pewter_swatch.jpg)|![](./returned_colors/iridescent_pewter_returned.jpg)|
|Iridescent Silver|#a69e9e|[166, 158, 158]|![](./images/iridescent_silver_swatch.jpg)|![](./returned_colors/iridescent_silver_returned.jpg)|
|Italian Black Roman Earth|#212422|[33, 36, 34]|![](./images/italian_black_roman_earth_swatch.jpg)|![](./returned_colors/italian_black_roman_earth_returned.jpg)|
|Italian Burnt Sienna|#964511|[150, 69, 17]|![](./images/italian_burnt_sienna_swatch.jpg)|![](./returned_colors/italian_burnt_sienna_returned.jpg)|
|Italian Green Ochre|#7d643b|[125, 100, 59]|![](./images/italian_green_ochre_swatch.jpg)|![](./returned_colors/italian_green_ochre_returned.jpg)|
|Italian Lemon Ochre|#d8b353|[216, 179, 83]|![](./images/italian_lemon_ochre_swatch.jpg)|![](./returned_colors/italian_lemon_ochre_returned.jpg)|
|Italian Orange Ochre|#be7421|[190, 116, 33]|![](./images/italian_orange_ochre_swatch.jpg)|![](./returned_colors/italian_orange_ochre_returned.jpg)|
|Italian Pink|#433631|[67, 54, 49]|![](./images/italian_pink_swatch.jpg)|![](./returned_colors/italian_pink_returned.jpg)|
|Italian Pompeii Red|#b3450e|[179, 69, 14]|![](./images/italian_pompeii_red_swatch.jpg)|![](./returned_colors/italian_pompeii_red_returned.jpg)|
|Italian Pozzuoli Earth|#993f19|[153, 63, 25]|![](./images/italian_pozzuoli_earth_swatch.jpg)|![](./returned_colors/italian_pozzuoli_earth_returned.jpg)|
|Italian Raw Sienna|#5f4018|[95, 64, 24]|![](./images/italian_raw_sienna_swatch.jpg)|![](./returned_colors/italian_raw_sienna_returned.jpg)|
|Italian Raw Umber|#81734f|[129, 115, 79]|![](./images/italian_raw_umber_swatch.jpg)|![](./returned_colors/italian_raw_umber_returned.jpg)|
|Italian Rosso Veneto|#b0622c|[176, 98, 44]|![](./images/italian_rosso_veneto_swatch.jpg)|![](./returned_colors/italian_rosso_veneto_returned.jpg)|
|Italian Terra Rosa|#7b361d|[123, 54, 29]|![](./images/italian_terra_rosa_swatch.jpg)|![](./returned_colors/italian_terra_rosa_returned.jpg)|
|Italian Terra Verte|#91a784|[145, 167, 132]|![](./images/italian_terra_verte_swatch.jpg)|![](./returned_colors/italian_terra_verte_returned.jpg)|
|Italian Yellow Ochre|#af8837|[175, 136, 55]|![](./images/italian_yellow_ochre_swatch.jpg)|![](./returned_colors/italian_yellow_ochre_returned.jpg)|
|Ivory Black|#2e3537|[46, 53, 55]|![](./images/ivory_black_swatch.jpg)|![](./returned_colors/ivory_black_returned.jpg)|
|Jaune Brilliant|#eebe69|[238, 190, 105]|![](./images/jaune_brilliant_swatch.jpg)|![](./returned_colors/jaune_brilliant_returned.jpg)|
|King's Blue|#4b8fc7|[75, 143, 199]|![](./images/king's_blue_swatch.jpg)|![](./returned_colors/king's_blue_returned.jpg)|
|Lamp Black|#2e3538|[46, 53, 56]|![](./images/lamp_black_swatch.jpg)|![](./returned_colors/lamp_black_returned.jpg)|
|Manganese Violet|#2f2340|[47, 35, 64]|![](./images/manganese_violet_swatch.jpg)|![](./returned_colors/manganese_violet_returned.jpg)|
|Mars Black|#10191b|[16, 25, 27]|![](./images/mars_black_swatch.jpg)|![](./returned_colors/mars_black_returned.jpg)|
|Mars Orange|#7c3e1f|[124, 62, 31]|![](./images/mars_orange_swatch.jpg)|![](./returned_colors/mars_orange_returned.jpg)|
|Mars Red|#501807|[80, 24, 7]|![](./images/mars_red_swatch.jpg)|![](./returned_colors/mars_red_returned.jpg)|
|Mars Red Light|#884a3b|[136, 74, 59]|![](./images/mars_red_light_swatch.jpg)|![](./returned_colors/mars_red_light_returned.jpg)|
|Mars Violet|#5d3732|[93, 55, 50]|![](./images/mars_violet_swatch.jpg)|![](./returned_colors/mars_violet_returned.jpg)|
|Mars Yellow Deep|#a77931|[167, 121, 49]|![](./images/mars_yellow_deep_swatch.jpg)|![](./returned_colors/mars_yellow_deep_returned.jpg)|
|Mars Yellow Light|#9a7435|[154, 116, 53]|![](./images/mars_yellow_light_swatch.jpg)|![](./returned_colors/mars_yellow_light_returned.jpg)|
|Montserrat Orange|#d6874c|[214, 135, 76]|![](./images/montserrat_orange_swatch.jpg)|![](./returned_colors/montserrat_orange_returned.jpg)|
|Naples Yellow|#d9b748|[217, 183, 72]|![](./images/naples_yellow_swatch.jpg)|![](./returned_colors/naples_yellow_returned.jpg)|
|Naples Yellow Italian|#e9bf50|[233, 191, 80]|![](./images/naples_yellow_italian_swatch.jpg)|![](./returned_colors/naples_yellow_italian_returned.jpg)|
|Naples Yellow Reddish|#d48f49|[212, 143, 73]|![](./images/naples_yellow_reddish_swatch.jpg)|![](./returned_colors/naples_yellow_reddish_returned.jpg)|
|Nickel Azo Yellow|#302c21|[48, 44, 33]|![](./images/nickel_azo_yellow_swatch.jpg)|![](./returned_colors/nickel_azo_yellow_returned.jpg)|
|Nickel Yellow|#e4d95e|[228, 217, 94]|![](./images/nickel_yellow_swatch.jpg)|![](./returned_colors/nickel_yellow_returned.jpg)|
|Olive Green|#4e6621|[78, 102, 33]|![](./images/olive_green_swatch.jpg)|![](./returned_colors/olive_green_returned.jpg)|
|Payne's Gray|#192128|[25, 33, 40]|![](./images/payne's_gray_swatch.jpg)|![](./returned_colors/payne's_gray_returned.jpg)|
|Payne's Gray (Violet)|#090e12|[9, 14, 18]|![](./images/payne's_gray_(violet)_swatch.jpg)|![](./returned_colors/payne's_gray_(violet)_returned.jpg)|
|Permanent Crimson|#76251f|[118, 37, 31]|![](./images/permanent_crimson_swatch.jpg)|![](./returned_colors/permanent_crimson_returned.jpg)|
|Permanent Green|#1b6331|[27, 99, 49]|![](./images/permanent_green_swatch.jpg)|![](./returned_colors/permanent_green_returned.jpg)|
|Permanent Green Light|#7dc66c|[125, 198, 108]|![](./images/permanent_green_light_swatch.jpg)|![](./returned_colors/permanent_green_light_returned.jpg)|
|Permanent Lemon|#ede44f|[237, 228, 79]|![](./images/permanent_lemon_swatch.jpg)|![](./returned_colors/permanent_lemon_returned.jpg)|
|Permanent Orange|#f7692a|[247, 105, 42]|![](./images/permanent_orange_swatch.jpg)|![](./returned_colors/permanent_orange_returned.jpg)|
|Permanent Red-Orange|#c14419|[193, 68, 25]|![](./images/permanent_red-orange_swatch.jpg)|![](./returned_colors/permanent_red-orange_returned.jpg)|
|Permanent Yellow Deep|#f2ac09|[242, 172, 9]|![](./images/permanent_yellow_deep_swatch.jpg)|![](./returned_colors/permanent_yellow_deep_returned.jpg)|
|Permanent Yellow Light|#f0e433|[240, 228, 51]|![](./images/permanent_yellow_light_swatch.jpg)|![](./returned_colors/permanent_yellow_light_returned.jpg)|
|Permanent Yellow Medium|#edd129|[237, 209, 41]|![](./images/permanent_yellow_medium_swatch.jpg)|![](./returned_colors/permanent_yellow_medium_returned.jpg)|
|Persian Rose|#de4c4b|[222, 76, 75]|![](./images/persian_rose_swatch.jpg)|![](./returned_colors/persian_rose_returned.jpg)|
|Perylene Crimson|#44211e|[68, 33, 30]|![](./images/perylene_crimson_swatch.jpg)|![](./returned_colors/perylene_crimson_returned.jpg)|
|Phthalo Blue|#1d2b5d|[29, 43, 93]|![](./images/phthalo_blue_swatch.jpg)|![](./returned_colors/phthalo_blue_returned.jpg)|
|Phthalo Green|#1a2b38|[26, 43, 56]|![](./images/phthalo_green_swatch.jpg)|![](./returned_colors/phthalo_green_returned.jpg)|
|Phthalo Green-Yellowish|#1d3f38|[29, 63, 56]|![](./images/phthalo_green-yellowish_swatch.jpg)|![](./returned_colors/phthalo_green-yellowish_returned.jpg)|
|Phthalo Turquoise|#194c5d|[25, 76, 93]|![](./images/phthalo_turquoise_swatch.jpg)|![](./returned_colors/phthalo_turquoise_returned.jpg)|
|Provence Violet Bluish|#372b76|[55, 43, 118]|![](./images/provence_violet_bluish_swatch.jpg)|![](./returned_colors/provence_violet_bluish_returned.jpg)|
|Provence Violet Reddish|#6f3258|[111, 50, 88]|![](./images/provence_violet_reddish_swatch.jpg)|![](./returned_colors/provence_violet_reddish_returned.jpg)|
|Prussian Blue|#0e203a|[14, 32, 58]|![](./images/prussian_blue_swatch.jpg)|![](./returned_colors/prussian_blue_returned.jpg)|
|Pyrrole Orange|#fd6107|[253, 97, 7]|![](./images/pyrrole_orange_swatch.jpg)|![](./returned_colors/pyrrole_orange_returned.jpg)|
|Pyrrole Red|#a70201|[167, 2, 1]|![](./images/pyrrole_red_swatch.jpg)|![](./returned_colors/pyrrole_red_returned.jpg)|
|Quinacridone Gold Brown|#593330|[89, 51, 48]|![](./images/quinacridone_gold_brown_swatch.jpg)|![](./returned_colors/quinacridone_gold_brown_returned.jpg)|
|Quinacridone Magenta|#541e18|[84, 30, 24]|![](./images/quinacridone_magenta_swatch.jpg)|![](./returned_colors/quinacridone_magenta_returned.jpg)|
|Quinacridone Red|#a43232|[164, 50, 50]|![](./images/quinacridone_red_swatch.jpg)|![](./returned_colors/quinacridone_red_returned.jpg)|
|Quinacridone Violet|#582127|[88, 33, 39]|![](./images/quinacridone_violet_swatch.jpg)|![](./returned_colors/quinacridone_violet_returned.jpg)|
|Raw Sienna|#9e733a|[158, 115, 58]|![](./images/raw_sienna_swatch.jpg)|![](./returned_colors/raw_sienna_returned.jpg)|
|Raw Umber|#222620|[34, 38, 32]|![](./images/raw_umber_swatch.jpg)|![](./returned_colors/raw_umber_returned.jpg)|
|Red Ochre|#65331f|[101, 51, 31]|![](./images/red_ochre_swatch.jpg)|![](./returned_colors/red_ochre_returned.jpg)|
|Red Umber|#180d05|[24, 13, 5]|![](./images/red_umber_swatch.jpg)|![](./returned_colors/red_umber_returned.jpg)|
|SF Cerulean Blue French|#273675|[39, 54, 117]|![](./images/sf_cerulean_blue_french_swatch.jpg)|![](./returned_colors/sf_cerulean_blue_french_returned.jpg)|
|SF Cobalt Violet Light|#ac3fab|[172, 63, 171]|![](./images/sf_cobalt_violet_light_swatch.jpg)|![](./returned_colors/sf_cobalt_violet_light_returned.jpg)|
|SF Flake White|#4d5660|[77, 86, 96]|![](./images/sf_flake_white_swatch.jpg)|![](./returned_colors/sf_flake_white_returned.jpg)|
|SF French Ardoise Grey|#827b6c|[130, 123, 108]|![](./images/sf_french_ardoise_grey_swatch.jpg)|![](./returned_colors/sf_french_ardoise_grey_returned.jpg)|
|SF Italian Terra Verte|#374d41|[55, 77, 65]|![](./images/sf_italian_terra_verte_swatch.jpg)|![](./returned_colors/sf_italian_terra_verte_returned.jpg)|
|SF Porcelain White|#c4c2cb|[196, 194, 203]|![](./images/sf_porcelain_white_swatch.jpg)|![](./returned_colors/sf_porcelain_white_returned.jpg)|
|SF Titanium White|#d9d8df|[217, 216, 223]|![](./images/sf_titanium_white_swatch.jpg)|![](./returned_colors/sf_titanium_white_returned.jpg)|
|SF Ultramarine Blue|#e7e5e4|[231, 229, 228]|![](./images/sf_ultramarine_blue_swatch.jpg)|![](./returned_colors/sf_ultramarine_blue_returned.jpg)|
|SF Ultramarine Blue French|#232679|[35, 38, 121]|![](./images/sf_ultramarine_blue_french_swatch.jpg)|![](./returned_colors/sf_ultramarine_blue_french_returned.jpg)|
|SF Ultramarine Pink|#583046|[88, 48, 70]|![](./images/sf_ultramarine_pink_swatch.jpg)|![](./returned_colors/sf_ultramarine_pink_returned.jpg)|
|SF Ultramarine Violet|#272a41|[39, 42, 65]|![](./images/sf_ultramarine_violet_swatch.jpg)|![](./returned_colors/sf_ultramarine_violet_returned.jpg)|
|Sap Green|#2c4030|[44, 64, 48]|![](./images/sap_green_swatch.jpg)|![](./returned_colors/sap_green_returned.jpg)|
|Sevres Blue|#0657a6|[6, 87, 166]|![](./images/sevres_blue_swatch.jpg)|![](./returned_colors/sevres_blue_returned.jpg)|
|Spanish Earth|#4f332b|[79, 51, 43]|![](./images/spanish_earth_swatch.jpg)|![](./returned_colors/spanish_earth_returned.jpg)|
|Stil De Grain|#534539|[83, 69, 57]|![](./images/stil_de_grain_swatch.jpg)|![](./returned_colors/stil_de_grain_returned.jpg)|
|Titan Buff|#e0d1c2|[224, 209, 194]|![](./images/titan_buff_swatch.jpg)|![](./returned_colors/titan_buff_returned.jpg)|
|Titanium - Zinc White|#e7e4d2|[231, 228, 210]|![](./images/titanium_-_zinc_white_swatch.jpg)|![](./returned_colors/titanium_-_zinc_white_returned.jpg)|
|Titanium White|#f3f1df|[243, 241, 223]|![](./images/titanium_white_swatch.jpg)|![](./returned_colors/titanium_white_returned.jpg)|
|Transparent Red Iron Oxide|#2f151e|[47, 21, 30]|![](./images/transparent_red_iron_oxide_swatch.jpg)|![](./returned_colors/transparent_red_iron_oxide_returned.jpg)|
|Transparent Yellow Iron Oxide|#22171b|[34, 23, 27]|![](./images/transparent_yellow_iron_oxide_swatch.jpg)|![](./returned_colors/transparent_yellow_iron_oxide_returned.jpg)|
|Turkey Umber|#161f1b|[22, 31, 27]|![](./images/turkey_umber_swatch.jpg)|![](./returned_colors/turkey_umber_returned.jpg)|
|Turquoise|#1d6e74|[29, 110, 116]|![](./images/turquoise_swatch.jpg)|![](./returned_colors/turquoise_returned.jpg)|
|Ultramarine Blue|#202943|[32, 41, 67]|![](./images/ultramarine_blue_swatch.jpg)|![](./returned_colors/ultramarine_blue_returned.jpg)|
|Ultramarine Blue French|#172057|[23, 32, 87]|![](./images/ultramarine_blue_french_swatch.jpg)|![](./returned_colors/ultramarine_blue_french_returned.jpg)|
|Ultramarine Pink|#4a2437|[74, 36, 55]|![](./images/ultramarine_pink_swatch.jpg)|![](./returned_colors/ultramarine_pink_returned.jpg)|
|Ultramarine Violet|#1a1941|[26, 25, 65]|![](./images/ultramarine_violet_swatch.jpg)|![](./returned_colors/ultramarine_violet_returned.jpg)|
|Unbleached Titanium|#d2bc95|[210, 188, 149]|![](./images/unbleached_titanium_swatch.jpg)|![](./returned_colors/unbleached_titanium_returned.jpg)|
|Unbleached Titanium Pale|#ddccae|[221, 204, 174]|![](./images/unbleached_titanium_pale_swatch.jpg)|![](./returned_colors/unbleached_titanium_pale_returned.jpg)|
|Van Dyke Brown|#39423b|[57, 66, 59]|![](./images/van_dyke_brown_swatch.jpg)|![](./returned_colors/van_dyke_brown_returned.jpg)|
|Veronese Green|#1f7b62|[31, 123, 98]|![](./images/veronese_green_swatch.jpg)|![](./returned_colors/veronese_green_returned.jpg)|
|Viridian|#284d4e|[40, 77, 78]|![](./images/viridian_swatch.jpg)|![](./returned_colors/viridian_returned.jpg)|
|Yellow Ochre (Domestic)|#b38533|[179, 133, 51]|![](./images/yellow_ochre_(domestic)_swatch.jpg)|![](./returned_colors/yellow_ochre_(domestic)_returned.jpg)|
|Yellow Ochre Burnt|#755b3d|[117, 91, 61]|![](./images/yellow_ochre_burnt_swatch.jpg)|![](./returned_colors/yellow_ochre_burnt_returned.jpg)|
|Zinc White|#f7f5de|[247, 245, 222]|![](./images/zinc_white_swatch.jpg)|![](./returned_colors/zinc_white_returned.jpg)|