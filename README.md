# Finding the Hex and RGB values for Williamsburg Oil Paints

## Introduction
The idea for this project came from a conversation I had with my cousin, who was working on a design project and wanted to get my input on colors to use for a user interface. As a painter, my mind works more in oil paint colors than it does in hex or RGB colors. 

Following our conversation, I decided to create a program that would gather all of the oil paint swatch images from the website of my favorite oil paint company, [Williamsburg Oils](https://www.williamsburgoils.com), and process each image, finding the median hex and RGB values within the image using computer vision and KMeans clustering. 

The end result is the table at the end of this README, where I've listed the hex color and corresponding RGB color next to the original image pulled from Williamsburg Oils' website. 

Please note that the resulting hex/RGB color resulting from the program is simply the median value derived from the KMeans clustering program, and is unlikely to represent an exact match to the color due to the transparent/opaque properties of oil paints. 

## Method



## Color List
|Color Name|Hex color|RGB Color|Paint swatch|
|-----|-----|-----|-----|
|Brilliant Yellow Extra Pale|#f4f0d4|[244, 240, 212]|![](./images/brilliant_yellow_extra_pale_swatch.jpg)|
|Brilliant Yellow Pale|#f4eca0|[244, 236, 160]|![](./images/brilliant_yellow_pale_swatch.jpg)|
|Nickel Yellow|#e7dd69|[231, 221, 105]|![](./images/nickel_yellow_swatch.jpg)|
|Bismuth Vanadate Yellow|#f4dd0c|[244, 221, 12]|![](./images/bismuth_vanadate_yellow_swatch.jpg)|
|Cadmium Lemon|#ebde33|[235, 222, 51]|![](./images/cadmium_lemon_swatch.jpg)|
|Permanent Lemon|#ece12f|[236, 225, 47]|![](./images/permanent_lemon_swatch.jpg)|
|Cadmium Yellow Light|#f0de28|[240, 222, 40]|![](./images/cadmium_yellow_light_swatch.jpg)|
|Permanent Yellow Light|#ede133|[237, 225, 51]|![](./images/permanent_yellow_light_swatch.jpg)|
|Cadmium Yellow Medium|#f1d220|[241, 210, 32]|![](./images/cadmium_yellow_medium_swatch.jpg)|
|Permanent Yellow Medium|#eed129|[238, 209, 41]|![](./images/permanent_yellow_medium_swatch.jpg)|
|Cadmium Yellow Deep|#eeb913|[238, 185, 19]|![](./images/cadmium_yellow_deep_swatch.jpg)|
|Permanent Yellow Deep|#f3ab13|[243, 171, 19]|![](./images/permanent_yellow_deep_swatch.jpg)|
|Cadmium Yellow Extra Deep|#f6940c|[246, 148, 12]|![](./images/cadmium_yellow_extra_deep_swatch.jpg)|
|Naples Yellow Italian|#e9c054|[233, 192, 84]|![](./images/naples_yellow_italian_swatch.jpg)|
|Naples Yellow|#cfb151|[207, 177, 81]|![](./images/naples_yellow_swatch.jpg)|
|Naples Yellow Reddish|#dd9951|[221, 153, 81]|![](./images/naples_yellow_reddish_swatch.jpg)|
|Canton Rose|#c97e5f|[201, 126, 95]|![](./images/canton_rose_swatch.jpg)|
|Jaune Brilliant|#ecbd6a|[236, 189, 106]|![](./images/jaune_brilliant_swatch.jpg)|
|Montserrat Orange|#d98e55|[217, 142, 85]|![](./images/montserrat_orange_swatch.jpg)|
|Cobalt Yellow|#d8b223|[216, 178, 35]|![](./images/cobalt_yellow_swatch.jpg)|
|Alizarin Yellow|#956a22|[149, 106, 34]|![](./images/alizarin_yellow_swatch.jpg)|
|Indian Yellow|#e1900a|[225, 144, 10]|![](./images/indian_yellow_swatch.jpg)|
|Unbleached Titanium Pale|#dbc9aa|[219, 201, 170]|![](./images/unbleached_titanium_pale_swatch.jpg)|
|Unbleached Titanium|#cdb792|[205, 183, 146]|![](./images/unbleached_titanium_swatch.jpg)|
|Cadmium Orange|#ee7e19|[238, 126, 25]|![](./images/cadmium_orange_swatch.jpg)|
|Permanent Orange|#f76524|[247, 101, 36]|![](./images/permanent_orange_swatch.jpg)|
|Alizarin Orange|#b25417|[178, 84, 23]|![](./images/alizarin_orange_swatch.jpg)|
|Permanent Red-Orange|#c6491c|[198, 73, 28]|![](./images/permanent_red-orange_swatch.jpg)|
|Pyrrole Orange|#f75903|[247, 89, 3]|![](./images/pyrrole_orange_swatch.jpg)|
|Cadmium Red Vermillion|#d74b1f|[215, 75, 31]|![](./images/cadmium_red_vermillion_swatch.jpg)|
|Cadmium Red Light|#e05319|[224, 83, 25]|![](./images/cadmium_red_light_swatch.jpg)|
|Fanchon Red|#c23a21|[194, 58, 33]|![](./images/fanchon_red_swatch.jpg)|
|Pyrrole Red|#b71a15|[183, 26, 21]|![](./images/pyrrole_red_swatch.jpg)|
|Cadmium Red Medium|#af3923|[175, 57, 35]|![](./images/cadmium_red_medium_swatch.jpg)|
|Cadmium Red Deep|#8b2f22|[139, 47, 34]|![](./images/cadmium_red_deep_swatch.jpg)|
|Cadmium Red Purple|#6d2a20|[109, 42, 32]|![](./images/cadmium_red_purple_swatch.jpg)|
|Cadmium Purple|#583233|[88, 50, 51]|![](./images/cadmium_purple_swatch.jpg)|
|Quinacridone Red|#a12e24|[161, 46, 36]|![](./images/quinacridone_red_swatch.jpg)|
|Quinacridone Magenta|#542223|[84, 34, 35]|![](./images/quinacridone_magenta_swatch.jpg)|
|Carl's Crimson (Permanent)|#642622|[100, 38, 34]|![](./images/carl's_crimson_(permanent)_swatch.jpg)|
|Permanent Crimson|#581f1a|[88, 31, 26]|![](./images/permanent_crimson_swatch.jpg)|
|Alizarin Crimson|#542223|[84, 34, 35]|![](./images/alizarin_crimson_swatch.jpg)|
|Ultramarine Pink|#371d2c|[55, 29, 44]|![](./images/ultramarine_pink_swatch.jpg)|
|Quinacridone Violet|#4c2029|[76, 32, 41]|![](./images/quinacridone_violet_swatch.jpg)|
|Perylene Crimson|#471d1d|[71, 29, 29]|![](./images/perylene_crimson_swatch.jpg)|
|Persian Rose|#dd4947|[221, 73, 71]|![](./images/persian_rose_swatch.jpg)|
|Dianthus Pink|#e9a2ad|[233, 162, 173]|![](./images/dianthus_pink_swatch.jpg)|
|Cobalt Violet Light|#722153|[114, 33, 83]|![](./images/cobalt_violet_light_swatch.jpg)|
|Cobalt Violet Deep|#2f1e51|[47, 30, 81]|![](./images/cobalt_violet_deep_swatch.jpg)|
|Provence Violet Reddish|#662851|[102, 40, 81]|![](./images/provence_violet_reddish_swatch.jpg)|
|Provence Violet Bluish|#332674|[51, 38, 116]|![](./images/provence_violet_bluish_swatch.jpg)|
|Manganese Violet|#322246|[50, 34, 70]|![](./images/manganese_violet_swatch.jpg)|
|Ultramarine Violet|#202141|[32, 33, 65]|![](./images/ultramarine_violet_swatch.jpg)|
|Egyptian Violet|#1b1a2d|[27, 26, 45]|![](./images/egyptian_violet_swatch.jpg)|
|King's Blue|#5d9acf|[93, 154, 207]|![](./images/king's_blue_swatch.jpg)|
|Sevres Blue|#1f6bb7|[31, 107, 183]|![](./images/sevres_blue_swatch.jpg)|
|Indigo|#18272d|[24, 39, 45]|![](./images/indigo_swatch.jpg)|
|Cerulean Blue (Genuine)|#1a4384|[26, 67, 132]|![](./images/cerulean_blue_(genuine)_swatch.jpg)|
|Cobalt Teal Greenish|#4da695|[77, 166, 149]|![](./images/cobalt_teal_greenish_swatch.jpg)|
|Cobalt Teal Bluish|#13a695|[19, 166, 149]|![](./images/cobalt_teal_bluish_swatch.jpg)|
|Cobalt Turqoise Greenish|#2a5a71|[42, 90, 113]|![](./images/cobalt_turqoise_greenish_swatch.jpg)|
|Cobalt Turqoise Bluish|#203c70|[32, 60, 112]|![](./images/cobalt_turqoise_bluish_swatch.jpg)|
|Ultramarine Blue|#162040|[22, 32, 64]|![](./images/ultramarine_blue_swatch.jpg)|
|Cobalt Blue|#16297e|[22, 41, 126]|![](./images/cobalt_blue_swatch.jpg)|
|Cobalt Blue Deep|#1b2a81|[27, 42, 129]|![](./images/cobalt_blue_deep_swatch.jpg)|
|Ultramarine Blue French|#182247|[24, 34, 71]|![](./images/ultramarine_blue_french_swatch.jpg)|
|Indanthrone Blue|#0b1246|[11, 18, 70]|![](./images/indanthrone_blue_swatch.jpg)|
|Prussian Blue|#0e1b26|[14, 27, 38]|![](./images/prussian_blue_swatch.jpg)|
|Phthalo Blue|#162857|[22, 40, 87]|![](./images/phthalo_blue_swatch.jpg)|
|Phthalo Turquoise|#112834|[17, 40, 52]|![](./images/phthalo_turquoise_swatch.jpg)|
|Cerulean Blue French|#132f70|[19, 47, 112]|![](./images/cerulean_blue_french_swatch.jpg)|
|Courbet Green|#1a2923|[26, 41, 35]|![](./images/courbet_green_swatch.jpg)|
|Turquoise|#1a6b70|[26, 107, 112]|![](./images/turquoise_swatch.jpg)|
|Veronese Green|#23846a|[35, 132, 106]|![](./images/veronese_green_swatch.jpg)|
|Cinnabar Green Light|#b6b432|[182, 180, 50]|![](./images/cinnabar_green_light_swatch.jpg)|
|Cadmium Green Light|#6c9636|[108, 150, 54]|![](./images/cadmium_green_light_swatch.jpg)|
|Permanent Green Light|#57b352|[87, 179, 82]|![](./images/permanent_green_light_swatch.jpg)|
|Permanent Green|#17612d|[23, 97, 45]|![](./images/permanent_green_swatch.jpg)|
|Cobalt Green|#2f6531|[47, 101, 49]|![](./images/cobalt_green_swatch.jpg)|
|Viridian|#1a3237|[26, 50, 55]|![](./images/viridian_swatch.jpg)|
|Phthalo Green-Yellowish|#14282c|[20, 40, 44]|![](./images/phthalo_green-yellowish_swatch.jpg)|
|Phthalo Green|#122633|[18, 38, 51]|![](./images/phthalo_green_swatch.jpg)|
|Sap Green|#273b29|[39, 59, 41]|![](./images/sap_green_swatch.jpg)|
|Cadmium Green|#3b6925|[59, 105, 37]|![](./images/cadmium_green_swatch.jpg)|
|Chromium Oxide Green|#517339|[81, 115, 57]|![](./images/chromium_oxide_green_swatch.jpg)|
|Olive Green|#4f671b|[79, 103, 27]|![](./images/olive_green_swatch.jpg)|
|Bohemian Green Earth|#353821|[53, 56, 33]|![](./images/bohemian_green_earth_swatch.jpg)|
|Earth Green|#323b1d|[50, 59, 29]|![](./images/earth_green_swatch.jpg)|
|Green Gold|#23310e|[35, 49, 14]|![](./images/green_gold_swatch.jpg)|
|Mars Violet|#4d241e|[77, 36, 30]|![](./images/mars_violet_swatch.jpg)|
|Titan Buff|#e7d8ca|[231, 216, 202]|![](./images/titan_buff_swatch.jpg)|
|Transparent Yellow Iron Oxide|#371b1c|[55, 27, 28]|![](./images/transparent_yellow_iron_oxide_swatch.jpg)|
|Yellow Ochre (Domestic)|#ae802b|[174, 128, 43]|![](./images/yellow_ochre_(domestic)_swatch.jpg)|
|Raw Sienna|#895f25|[137, 95, 37]|![](./images/raw_sienna_swatch.jpg)|
|Cyprus Orange|#955b26|[149, 91, 38]|![](./images/cyprus_orange_swatch.jpg)|
|Stil De Grain|#3a2f24|[58, 47, 36]|![](./images/stil_de_grain_swatch.jpg)|
|Transparent Red Iron Oxide|#261921|[38, 25, 33]|![](./images/transparent_red_iron_oxide_swatch.jpg)|
|Brown Pink|#272320|[39, 35, 32]|![](./images/brown_pink_swatch.jpg)|
|Quinacridone Gold Brown|#411c1a|[65, 28, 26]|![](./images/quinacridone_gold_brown_swatch.jpg)|
|Italian Pink|#302520|[48, 37, 32]|![](./images/italian_pink_swatch.jpg)|
|Burnt Sienna|#583122|[88, 49, 34]|![](./images/burnt_sienna_swatch.jpg)|
|Yellow Ochre Burnt|#5c4322|[92, 67, 34]|![](./images/yellow_ochre_burnt_swatch.jpg)|
|Brown Ochre|#5e4821|[94, 72, 33]|![](./images/brown_ochre_swatch.jpg)|
|Nickel Azo Yellow|#2d241a|[45, 36, 26]|![](./images/nickel_azo_yellow_swatch.jpg)|
|Red Ochre|#6c3b27|[108, 59, 39]|![](./images/red_ochre_swatch.jpg)|
|Spanish Earth|#4c2f27|[76, 47, 39]|![](./images/spanish_earth_swatch.jpg)|
|Mars Yellow Light|#a07a3a|[160, 122, 58]|![](./images/mars_yellow_light_swatch.jpg)|
|Mars Yellow Deep|#9f7127|[159, 113, 39]|![](./images/mars_yellow_deep_swatch.jpg)|
|Mars Orange|#7e4227|[126, 66, 39]|![](./images/mars_orange_swatch.jpg)|
|Mars Red Light|#763926|[118, 57, 38]|![](./images/mars_red_light_swatch.jpg)|
|Mars Red|#5f281d|[95, 40, 29]|![](./images/mars_red_swatch.jpg)|
|Burnt Umber|#27261f|[39, 38, 31]|![](./images/burnt_umber_swatch.jpg)|
|Dutch Brown (Transparent)|#1e1e1e|[30, 30, 30]|![](./images/dutch_brown_(transparent)_swatch.jpg)|
|Raw Umber|#1f231d|[31, 35, 29]|![](./images/raw_umber_swatch.jpg)|
|Turkey Umber|#1f2824|[31, 40, 36]|![](./images/turkey_umber_swatch.jpg)|
|Red Umber|#322923|[50, 41, 35]|![](./images/red_umber_swatch.jpg)|
|Van Dyke Brown|#2d3630|[45, 54, 48]|![](./images/van_dyke_brown_swatch.jpg)|
|Brown Umber|#282520|[40, 37, 32]|![](./images/brown_umber_swatch.jpg)|
|German Earth|#171c1b|[23, 28, 27]|![](./images/german_earth_swatch.jpg)|
|Mars Black|#141d1f|[20, 29, 31]|![](./images/mars_black_swatch.jpg)|
|Ivory Black|#191e20|[25, 30, 32]|![](./images/ivory_black_swatch.jpg)|
|Davy's Grey Deep|#222725|[34, 39, 37]|![](./images/davy's_grey_deep_swatch.jpg)|
|Graphite Gray|#30322e|[48, 50, 46]|![](./images/graphite_gray_swatch.jpg)|
|Payne's Gray (Violet)|#1d2126|[29, 33, 38]|![](./images/payne's_gray_(violet)_swatch.jpg)|
|Payne's Gray|#171f27|[23, 31, 39]|![](./images/payne's_gray_swatch.jpg)|
|Lamp Black|#1b2122|[27, 33, 34]|![](./images/lamp_black_swatch.jpg)|
|Cold Black|#182023|[24, 32, 35]|![](./images/cold_black_swatch.jpg)|
|Flake White|#f7f3d6|[247, 243, 214]|![](./images/flake_white_swatch.jpg)|
|Titanium - Zinc White|#f7f4df|[247, 244, 223]|![](./images/titanium_-_zinc_white_swatch.jpg)|
|Zinc White|#f6f4d9|[246, 244, 217]|![](./images/zinc_white_swatch.jpg)|
|Titanium White|#f5f2e1|[245, 242, 225]|![](./images/titanium_white_swatch.jpg)|
|French Terre Verte|#517665|[81, 118, 101]|![](./images/french_terre_verte_swatch.jpg)|
|French Yellow Ochre Deep|#9e6e2d|[158, 110, 45]|![](./images/french_yellow_ochre_deep_swatch.jpg)|
|French Raw Sienna|#896332|[137, 99, 50]|![](./images/french_raw_sienna_swatch.jpg)|
|French Ochre Havane|#9e6739|[158, 103, 57]|![](./images/french_ochre_havane_swatch.jpg)|
|French Rouge Indian|#733f2f|[115, 63, 47]|![](./images/french_rouge_indian_swatch.jpg)|
|French Brown Ochre|#4b3b2a|[75, 59, 42]|![](./images/french_brown_ochre_swatch.jpg)|
|French Burnt Ochre|#3e3024|[62, 48, 36]|![](./images/french_burnt_ochre_swatch.jpg)|
|French Burnt Umber|#312f29|[49, 47, 41]|![](./images/french_burnt_umber_swatch.jpg)|
|French Light Sienna|#6a5b35|[106, 91, 53]|![](./images/french_light_sienna_swatch.jpg)|
|French Ardoise Gray|#8a806b|[138, 128, 107]|![](./images/french_ardoise_gray_swatch.jpg)|
|French Raw Umber|#48422f|[72, 66, 47]|![](./images/french_raw_umber_swatch.jpg)|
|Italian Terra Verte|#4d6c47|[77, 108, 71]|![](./images/italian_terra_verte_swatch.jpg)|
|Italian Lemon Ochre|#c29527|[194, 149, 39]|![](./images/italian_lemon_ochre_swatch.jpg)|
|Italian Yellow Ochre|#ab8129|[171, 129, 41]|![](./images/italian_yellow_ochre_swatch.jpg)|
|Italian Raw Sienna|#7d5624|[125, 86, 36]|![](./images/italian_raw_sienna_swatch.jpg)|
|Italian Green Ochre|#73582b|[115, 88, 43]|![](./images/italian_green_ochre_swatch.jpg)|
|Italian Orange Ochre|#8f5220|[143, 82, 32]|![](./images/italian_orange_ochre_swatch.jpg)|
|Italian Pompeii Red|#9c4a2b|[156, 74, 43]|![](./images/italian_pompeii_red_swatch.jpg)|
|Italian Rosso Veneto|#854a2a|[133, 74, 42]|![](./images/italian_rosso_veneto_swatch.jpg)|
|Italian Pozzuoli Earth|#884123|[136, 65, 35]|![](./images/italian_pozzuoli_earth_swatch.jpg)|
|Italian Terra Rosa|#883f24|[136, 63, 36]|![](./images/italian_terra_rosa_swatch.jpg)|
|Italian Burnt Sienna|#63341c|[99, 52, 28]|![](./images/italian_burnt_sienna_swatch.jpg)|
|Italian Raw Umber|#3a3829|[58, 56, 41]|![](./images/italian_raw_umber_swatch.jpg)|
|Italian Black Roman Earth|#1f2322|[31, 35, 34]|![](./images/italian_black_roman_earth_swatch.jpg)|
|SF Flake White|#deddde|[222, 221, 222]|![](./images/sf_flake_white_swatch.jpg)|
|SF Porcelain White|#d4d2d8|[212, 210, 216]|![](./images/sf_porcelain_white_swatch.jpg)|
|SF Titanium White|#dcdbe1|[220, 219, 225]|![](./images/sf_titanium_white_swatch.jpg)|
|SF French Ardoise Grey|#8d867a|[141, 134, 122]|![](./images/sf_french_ardoise_grey_swatch.jpg)|
|SF Ultramarine Pink|#663853|[102, 56, 83]|![](./images/sf_ultramarine_pink_swatch.jpg)|
|SF Cobalt Violet Light|#893298|[137, 50, 152]|![](./images/sf_cobalt_violet_light_swatch.jpg)|
|SF Ultramarine Violet|#2a2a4e|[42, 42, 78]|![](./images/sf_ultramarine_violet_swatch.jpg)|
|SF Cerulean Blue French|#273570|[39, 53, 112]|![](./images/sf_cerulean_blue_french_swatch.jpg)|
|SF Ultramarine Blue|#1f235a|[31, 35, 90]|![](./images/sf_ultramarine_blue_swatch.jpg)|
|SF Ultramarine Blue French|#25285a|[37, 40, 90]|![](./images/sf_ultramarine_blue_french_swatch.jpg)|
|SF Italian Terra Verte|#3c5444|[60, 84, 68]|![](./images/sf_italian_terra_verte_swatch.jpg)|
|Iridescent Copper|#914b31|[145, 75, 49]|![](./images/iridescent_copper_swatch.jpg)|
|Iridescent Pale Gold|#eac66e|[234, 198, 110]|![](./images/iridescent_pale_gold_swatch.jpg)|
|Iridescent Pearl White|#e4ddc9|[228, 221, 201]|![](./images/iridescent_pearl_white_swatch.jpg)|
|Iridescent Bronze|#786644|[120, 102, 68]|![](./images/iridescent_bronze_swatch.jpg)|
|Iridescent Silver|#7c7977|[124, 121, 119]|![](./images/iridescent_silver_swatch.jpg)|
|Iridescent Pewter|#666565|[102, 101, 101]|![](./images/iridescent_pewter_swatch.jpg)|
|Interference Violet|#c9b5b9|[201, 181, 185]|![](./images/interference_violet_swatch.jpg)|
|Interference Red|#d8ba9e|[216, 186, 158]|![](./images/interference_red_swatch.jpg)|
|Interference Blue|#b8c0c9|[184, 192, 201]|![](./images/interference_blue_swatch.jpg)|
|Interference Green|#dddbb5|[221, 219, 181]|![](./images/interference_green_swatch.jpg)|