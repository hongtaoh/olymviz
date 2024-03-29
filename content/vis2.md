---
title: Chnages in Female Particiation Across Continents
author: Chris Fang & Hongtao Hao
---
To visualize changes in female participation in each continent, we first used a simple line graph where we put all the continent together. The x-axis is time, and the y-axis is female participation. The legend shows the colors associated with the continents. See Figure 25.

<div id="figure27" class="vis"></div>
<div class="caption">Figure 25: Line graph for female participation by continent</div>

The graph was very messy. As there were six continents and one global average, we could not distinguish between the seven categories very easily. So we gave up this option. 

Then we tried a small multiple in which each continent and the global average were shown in simple line graphs. This chart showed every continent clearly but it was not very easy to make a comparison. See Figure 26.

<!--
[**FIGURE 28 HERE**]

{{<figure src="/pics/g-2-2.png" caption="Line graph in small multiple for female participation by continent" style="min-width: 100%">}}

The above visualization was made by seaborn. It's not of high resolution, so we tried altair for:

-->

<div id="figure28_2" class="vis"></div>
<div class="caption">Figure 26: Line graph in small multiple for female participation by continent</div>

To make comparisons clearer, we decided to use an area chart. We stacked each area chart each representing a continent along a vertical line. However, comparisons were still difficult. Most importantly, in terms of using color as the visual encoding, this graph has too many categories. Besides, it has red and green at the same time, and therefore is not accessible to colorblind populations. See Figure 27.

<!--

{{<figure src="/pics/g-2-3.png" caption="Area chart in small multiple for female participation by continent" style="min-width: 110%">}}

-->

<div id="figure29" class="vis"></div>
<div class="caption">Figure 27: Stacked bar chart for female participation by continent</div>

We then went back to the small multiple. Since we cared about the comparison between each continent, we decided to plot every continent and the global average in each of the six graphs. We highlighted only one continent in each graph, and set all other continents grey in the background. It worked much better than out earlier attempts, but one drawback is that it did not allow comparison with the global average. See Figure 28.

{{<figure src="https://raw.githubusercontent.com/hongtaoh/olymvis-data/master/output/vis/g-2-5.png" class="fullwidth">}}
  
<div class="caption-up-a-little">Figure 28: Line graph in small multiple for female participation by continent against all other groups</div>

Finally, we decided to highlight the global average with a black line. This time, comparisons both between continents and with the global average were clear. See Figure 29.

{{<figure src="https://raw.githubusercontent.com/hongtaoh/olymvis-data/master/output/vis/g-2-6.png" class="fullwidth">}}
  
<div class="caption-up-a-little">Figure 29: Line graph in small multiple for female participation by continent against global statistics</div>

<script type="text/javascript">
var figure27 = {
  "$schema": "https://vega.github.io/schema/vega/v5.json",
  "background": "white",
  "padding": 5,
  "width": 700,
  "height": 300,
  "title": {
    "anchor": "middle",
    "text": "Changes in female athletes participation in Summer Olympics over time",
    "frame": "group"
  },
  "style": "cell",
  "data": [
    {"name": "selector010_store"},
    {
      "name": "data-c9cd4958aa454941ccfb344427499b56",
      "values": [
        {
          "Year": 1896,
          "Continent": "Global",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1900,
          "Continent": "Global",
          "Female_Percentage": 0.016045548654244308,
          "Female Percentage": "1.6%"
        },
        {
          "Year": 1904,
          "Continent": "Global",
          "Female_Percentage": 0.012307692307692308,
          "Female Percentage": "1.2%"
        },
        {
          "Year": 1906,
          "Continent": "Global",
          "Female_Percentage": 0.006489675516224189,
          "Female Percentage": "0.6%"
        },
        {
          "Year": 1908,
          "Continent": "Global",
          "Female_Percentage": 0.015568068896985756,
          "Female Percentage": "1.6%"
        },
        {
          "Year": 1912,
          "Continent": "Global",
          "Female_Percentage": 0.020242914979757085,
          "Female Percentage": "2.0%"
        },
        {
          "Year": 1920,
          "Continent": "Global",
          "Female_Percentage": 0.03247863247863248,
          "Female Percentage": "3.2%"
        },
        {
          "Year": 1924,
          "Continent": "Global",
          "Female_Percentage": 0.04917363803305448,
          "Female Percentage": "4.9%"
        },
        {
          "Year": 1928,
          "Continent": "Global",
          "Female_Percentage": 0.08397582829756199,
          "Female Percentage": "8.4%"
        },
        {
          "Year": 1932,
          "Continent": "Global",
          "Female_Percentage": 0.11859193438140808,
          "Female Percentage": "11.9%"
        },
        {
          "Year": 1936,
          "Continent": "Global",
          "Female_Percentage": 0.07177974434611603,
          "Female Percentage": "7.2%"
        },
        {
          "Year": 1948,
          "Continent": "Global",
          "Female_Percentage": 0.0974740932642487,
          "Female Percentage": "9.7%"
        },
        {
          "Year": 1952,
          "Continent": "Global",
          "Female_Percentage": 0.17301414581066374,
          "Female Percentage": "17.3%"
        },
        {
          "Year": 1956,
          "Continent": "Global",
          "Female_Percentage": 0.1704136690647482,
          "Female Percentage": "17.0%"
        },
        {
          "Year": 1960,
          "Continent": "Global",
          "Female_Percentage": 0.1761111111111111,
          "Female Percentage": "17.6%"
        },
        {
          "Year": 1964,
          "Continent": "Global",
          "Female_Percentage": 0.17183667580435724,
          "Female Percentage": "17.2%"
        },
        {
          "Year": 1968,
          "Continent": "Global",
          "Female_Percentage": 0.19755020652328728,
          "Female Percentage": "19.8%"
        },
        {
          "Year": 1972,
          "Continent": "Global",
          "Female_Percentage": 0.2010383965225791,
          "Female Percentage": "20.1%"
        },
        {
          "Year": 1976,
          "Continent": "Global",
          "Female_Percentage": 0.2333720592506535,
          "Female Percentage": "23.3%"
        },
        {
          "Year": 1980,
          "Continent": "Global",
          "Female_Percentage": 0.22398271516024487,
          "Female Percentage": "22.4%"
        },
        {
          "Year": 1984,
          "Continent": "Global",
          "Female_Percentage": 0.25244707489187346,
          "Female Percentage": "25.2%"
        },
        {
          "Year": 1988,
          "Continent": "Global",
          "Female_Percentage": 0.2830937035200793,
          "Female Percentage": "28.3%"
        },
        {
          "Year": 1992,
          "Continent": "Global",
          "Female_Percentage": 0.3129472457979697,
          "Female Percentage": "31.3%"
        },
        {
          "Year": 1996,
          "Continent": "Global",
          "Female_Percentage": 0.36325520654340493,
          "Female Percentage": "36.3%"
        },
        {
          "Year": 2000,
          "Continent": "Global",
          "Female_Percentage": 0.3939145299145299,
          "Female Percentage": "39.4%"
        },
        {
          "Year": 2004,
          "Continent": "Global",
          "Female_Percentage": 0.4132602893664841,
          "Female Percentage": "41.3%"
        },
        {
          "Year": 2008,
          "Continent": "Global",
          "Female_Percentage": 0.4284037558685446,
          "Female Percentage": "42.8%"
        },
        {
          "Year": 2012,
          "Continent": "Global",
          "Female_Percentage": 0.4500399100210435,
          "Female Percentage": "45.0%"
        },
        {
          "Year": 2016,
          "Continent": "Global",
          "Female_Percentage": 0.4535101729046594,
          "Female Percentage": "45.4%"
        },
        {
          "Year": 1896,
          "Continent": "Africa",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1900,
          "Continent": "Africa",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1904,
          "Continent": "Africa",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1906,
          "Continent": "Africa",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1908,
          "Continent": "Africa",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1912,
          "Continent": "Africa",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1920,
          "Continent": "Africa",
          "Female_Percentage": 0.01680672268907563,
          "Female Percentage": "1.7%"
        },
        {
          "Year": 1924,
          "Continent": "Africa",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1928,
          "Continent": "Africa",
          "Female_Percentage": 0.1411764705882353,
          "Female Percentage": "14.1%"
        },
        {
          "Year": 1932,
          "Continent": "Africa",
          "Female_Percentage": 0.25,
          "Female Percentage": "25.0%"
        },
        {
          "Year": 1936,
          "Continent": "Africa",
          "Female_Percentage": 0.1,
          "Female Percentage": "10.0%"
        },
        {
          "Year": 1948,
          "Continent": "Africa",
          "Female_Percentage": 0.009569377990430622,
          "Female Percentage": "1.0%"
        },
        {
          "Year": 1952,
          "Continent": "Africa",
          "Female_Percentage": 0.02735562310030395,
          "Female Percentage": "2.7%"
        },
        {
          "Year": 1956,
          "Continent": "Africa",
          "Female_Percentage": 0.0748663101604278,
          "Female Percentage": "7.5%"
        },
        {
          "Year": 1960,
          "Continent": "Africa",
          "Female_Percentage": 0.04456824512534819,
          "Female Percentage": "4.5%"
        },
        {
          "Year": 1964,
          "Continent": "Africa",
          "Female_Percentage": 0.045454545454545456,
          "Female Percentage": "4.5%"
        },
        {
          "Year": 1968,
          "Continent": "Africa",
          "Female_Percentage": 0.039886039886039885,
          "Female Percentage": "4.0%"
        },
        {
          "Year": 1972,
          "Continent": "Africa",
          "Female_Percentage": 0.056985294117647065,
          "Female Percentage": "5.7%"
        },
        {
          "Year": 1976,
          "Continent": "Africa",
          "Female_Percentage": 0.0707070707070707,
          "Female Percentage": "7.1%"
        },
        {
          "Year": 1980,
          "Continent": "Africa",
          "Female_Percentage": 0.1524590163934426,
          "Female Percentage": "15.2%"
        },
        {
          "Year": 1984,
          "Continent": "Africa",
          "Female_Percentage": 0.09419354838709676,
          "Female Percentage": "9.4%"
        },
        {
          "Year": 1988,
          "Continent": "Africa",
          "Female_Percentage": 0.13974799541809851,
          "Female Percentage": "14.0%"
        },
        {
          "Year": 1992,
          "Continent": "Africa",
          "Female_Percentage": 0.22341568206229864,
          "Female Percentage": "22.3%"
        },
        {
          "Year": 1996,
          "Continent": "Africa",
          "Female_Percentage": 0.2462077012835473,
          "Female Percentage": "24.6%"
        },
        {
          "Year": 2000,
          "Continent": "Africa",
          "Female_Percentage": 0.3296370967741936,
          "Female Percentage": "33.0%"
        },
        {
          "Year": 2004,
          "Continent": "Africa",
          "Female_Percentage": 0.33407572383073497,
          "Female Percentage": "33.4%"
        },
        {
          "Year": 2008,
          "Continent": "Africa",
          "Female_Percentage": 0.3874734607218684,
          "Female Percentage": "38.7%"
        },
        {
          "Year": 2012,
          "Continent": "Africa",
          "Female_Percentage": 0.399581589958159,
          "Female Percentage": "40.0%"
        },
        {
          "Year": 2016,
          "Continent": "Africa",
          "Female_Percentage": 0.3836772983114447,
          "Female Percentage": "38.4%"
        },
        {
          "Year": 1896,
          "Continent": "Asia",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1900,
          "Continent": "Asia",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1904,
          "Continent": "Asia",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1906,
          "Continent": "Asia",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1908,
          "Continent": "Asia",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1912,
          "Continent": "Asia",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1920,
          "Continent": "Asia",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1924,
          "Continent": "Asia",
          "Female_Percentage": 0.033707865168539325,
          "Female Percentage": "3.4%"
        },
        {
          "Year": 1928,
          "Continent": "Asia",
          "Female_Percentage": 0.015873015873015872,
          "Female Percentage": "1.6%"
        },
        {
          "Year": 1932,
          "Continent": "Asia",
          "Female_Percentage": 0.11203319502074688,
          "Female Percentage": "11.2%"
        },
        {
          "Year": 1936,
          "Continent": "Asia",
          "Female_Percentage": 0.057620817843866176,
          "Female Percentage": "5.8%"
        },
        {
          "Year": 1948,
          "Continent": "Asia",
          "Female_Percentage": 0.0069124423963133645,
          "Female Percentage": "0.7%"
        },
        {
          "Year": 1952,
          "Continent": "Asia",
          "Female_Percentage": 0.065439672801636,
          "Female Percentage": "6.5%"
        },
        {
          "Year": 1956,
          "Continent": "Asia",
          "Female_Percentage": 0.1060126582278481,
          "Female Percentage": "10.6%"
        },
        {
          "Year": 1960,
          "Continent": "Asia",
          "Female_Percentage": 0.129366106080207,
          "Female Percentage": "12.9%"
        },
        {
          "Year": 1964,
          "Continent": "Asia",
          "Female_Percentage": 0.14587593728698026,
          "Female Percentage": "14.6%"
        },
        {
          "Year": 1968,
          "Continent": "Asia",
          "Female_Percentage": 0.17119244391971666,
          "Female Percentage": "17.1%"
        },
        {
          "Year": 1972,
          "Continent": "Asia",
          "Female_Percentage": 0.14781746031746032,
          "Female Percentage": "14.8%"
        },
        {
          "Year": 1976,
          "Continent": "Asia",
          "Female_Percentage": 0.16761041902604756,
          "Female Percentage": "16.8%"
        },
        {
          "Year": 1980,
          "Continent": "Asia",
          "Female_Percentage": 0.1494661921708185,
          "Female Percentage": "14.9%"
        },
        {
          "Year": 1984,
          "Continent": "Asia",
          "Female_Percentage": 0.2409855769230769,
          "Female Percentage": "24.1%"
        },
        {
          "Year": 1988,
          "Continent": "Asia",
          "Female_Percentage": 0.3037466547725245,
          "Female Percentage": "30.4%"
        },
        {
          "Year": 1992,
          "Continent": "Asia",
          "Female_Percentage": 0.31186440677966104,
          "Female Percentage": "31.2%"
        },
        {
          "Year": 1996,
          "Continent": "Asia",
          "Female_Percentage": 0.3821571238348868,
          "Female Percentage": "38.2%"
        },
        {
          "Year": 2000,
          "Continent": "Asia",
          "Female_Percentage": 0.39642620780939775,
          "Female Percentage": "39.6%"
        },
        {
          "Year": 2004,
          "Continent": "Asia",
          "Female_Percentage": 0.4359058207979071,
          "Female Percentage": "43.6%"
        },
        {
          "Year": 2008,
          "Continent": "Asia",
          "Female_Percentage": 0.43423423423423424,
          "Female Percentage": "43.4%"
        },
        {
          "Year": 2012,
          "Continent": "Asia",
          "Female_Percentage": 0.4599396580623533,
          "Female Percentage": "46.0%"
        },
        {
          "Year": 2016,
          "Continent": "Asia",
          "Female_Percentage": 0.4653897849462366,
          "Female Percentage": "46.5%"
        },
        {
          "Year": 1896,
          "Continent": "Europe",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1900,
          "Continent": "Europe",
          "Female_Percentage": 0.012528473804100227,
          "Female Percentage": "1.3%"
        },
        {
          "Year": 1904,
          "Continent": "Europe",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1906,
          "Continent": "Europe",
          "Female_Percentage": 0.006905210295040804,
          "Female Percentage": "0.7%"
        },
        {
          "Year": 1908,
          "Continent": "Europe",
          "Female_Percentage": 0.01800076599004213,
          "Female Percentage": "1.8%"
        },
        {
          "Year": 1912,
          "Continent": "Europe",
          "Female_Percentage": 0.024897480960749854,
          "Female Percentage": "2.5%"
        },
        {
          "Year": 1920,
          "Continent": "Europe",
          "Female_Percentage": 0.03142943487458446,
          "Female Percentage": "3.1%"
        },
        {
          "Year": 1924,
          "Continent": "Europe",
          "Female_Percentage": 0.05149330587023687,
          "Female Percentage": "5.1%"
        },
        {
          "Year": 1928,
          "Continent": "Europe",
          "Female_Percentage": 0.0821664464993395,
          "Female Percentage": "8.2%"
        },
        {
          "Year": 1932,
          "Continent": "Europe",
          "Female_Percentage": 0.10588235294117647,
          "Female Percentage": "10.6%"
        },
        {
          "Year": 1936,
          "Continent": "Europe",
          "Female_Percentage": 0.06700091157702825,
          "Female Percentage": "6.7%"
        },
        {
          "Year": 1948,
          "Continent": "Europe",
          "Female_Percentage": 0.1073929961089494,
          "Female Percentage": "10.7%"
        },
        {
          "Year": 1952,
          "Continent": "Europe",
          "Female_Percentage": 0.20599325262949,
          "Female Percentage": "20.6%"
        },
        {
          "Year": 1956,
          "Continent": "Europe",
          "Female_Percentage": 0.20808451998162608,
          "Female Percentage": "20.8%"
        },
        {
          "Year": 1960,
          "Continent": "Europe",
          "Female_Percentage": 0.19808861859252824,
          "Female Percentage": "19.8%"
        },
        {
          "Year": 1964,
          "Continent": "Europe",
          "Female_Percentage": 0.19008009858287125,
          "Female Percentage": "19.0%"
        },
        {
          "Year": 1968,
          "Continent": "Europe",
          "Female_Percentage": 0.20454545454545456,
          "Female Percentage": "20.5%"
        },
        {
          "Year": 1972,
          "Continent": "Europe",
          "Female_Percentage": 0.22300968580203165,
          "Female Percentage": "22.3%"
        },
        {
          "Year": 1976,
          "Continent": "Europe",
          "Female_Percentage": 0.2362555720653789,
          "Female Percentage": "23.6%"
        },
        {
          "Year": 1980,
          "Continent": "Europe",
          "Female_Percentage": 0.257801108194809,
          "Female Percentage": "25.8%"
        },
        {
          "Year": 1984,
          "Continent": "Europe",
          "Female_Percentage": 0.2688271604938272,
          "Female Percentage": "26.9%"
        },
        {
          "Year": 1988,
          "Continent": "Europe",
          "Female_Percentage": 0.29081000743126084,
          "Female Percentage": "29.1%"
        },
        {
          "Year": 1992,
          "Continent": "Europe",
          "Female_Percentage": 0.3262682418346073,
          "Female Percentage": "32.6%"
        },
        {
          "Year": 1996,
          "Continent": "Europe",
          "Female_Percentage": 0.3664026677782409,
          "Female Percentage": "36.6%"
        },
        {
          "Year": 2000,
          "Continent": "Europe",
          "Female_Percentage": 0.38596989491621697,
          "Female Percentage": "38.6%"
        },
        {
          "Year": 2004,
          "Continent": "Europe",
          "Female_Percentage": 0.4022806004618938,
          "Female Percentage": "40.2%"
        },
        {
          "Year": 2008,
          "Continent": "Europe",
          "Female_Percentage": 0.4252481849162839,
          "Female Percentage": "42.5%"
        },
        {
          "Year": 2012,
          "Continent": "Europe",
          "Female_Percentage": 0.4477747502270663,
          "Female Percentage": "44.8%"
        },
        {
          "Year": 2016,
          "Continent": "Europe",
          "Female_Percentage": 0.4510353417406197,
          "Female Percentage": "45.1%"
        },
        {
          "Year": 1896,
          "Continent": "North America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1900,
          "Continent": "North America",
          "Female_Percentage": 0.05960264900662252,
          "Female Percentage": "6.0%"
        },
        {
          "Year": 1904,
          "Continent": "North America",
          "Female_Percentage": 0.013605442176870748,
          "Female Percentage": "1.4%"
        },
        {
          "Year": 1906,
          "Continent": "North America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1908,
          "Continent": "North America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1912,
          "Continent": "North America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1920,
          "Continent": "North America",
          "Female_Percentage": 0.03942652329749104,
          "Female Percentage": "3.9%"
        },
        {
          "Year": 1924,
          "Continent": "North America",
          "Female_Percentage": 0.05843071786310518,
          "Female Percentage": "5.8%"
        },
        {
          "Year": 1928,
          "Continent": "North America",
          "Female_Percentage": 0.11,
          "Female Percentage": "11.0%"
        },
        {
          "Year": 1932,
          "Continent": "North America",
          "Female_Percentage": 0.14641148325358852,
          "Female Percentage": "14.6%"
        },
        {
          "Year": 1936,
          "Continent": "North America",
          "Female_Percentage": 0.1221264367816092,
          "Female Percentage": "12.2%"
        },
        {
          "Year": 1948,
          "Continent": "North America",
          "Female_Percentage": 0.11932418162618795,
          "Female Percentage": "11.9%"
        },
        {
          "Year": 1952,
          "Continent": "North America",
          "Female_Percentage": 0.16042154566744732,
          "Female Percentage": "16.0%"
        },
        {
          "Year": 1956,
          "Continent": "North America",
          "Female_Percentage": 0.19484240687679086,
          "Female Percentage": "19.5%"
        },
        {
          "Year": 1960,
          "Continent": "North America",
          "Female_Percentage": 0.21568627450980396,
          "Female Percentage": "21.6%"
        },
        {
          "Year": 1964,
          "Continent": "North America",
          "Female_Percentage": 0.2101661779081134,
          "Female Percentage": "21.0%"
        },
        {
          "Year": 1968,
          "Continent": "North America",
          "Female_Percentage": 0.2272957889396245,
          "Female Percentage": "22.7%"
        },
        {
          "Year": 1972,
          "Continent": "North America",
          "Female_Percentage": 0.23755924170616116,
          "Female Percentage": "23.8%"
        },
        {
          "Year": 1976,
          "Continent": "North America",
          "Female_Percentage": 0.27378964941569284,
          "Female Percentage": "27.4%"
        },
        {
          "Year": 1980,
          "Continent": "North America",
          "Female_Percentage": 0.17372881355932204,
          "Female Percentage": "17.4%"
        },
        {
          "Year": 1984,
          "Continent": "North America",
          "Female_Percentage": 0.3223987698616094,
          "Female Percentage": "32.2%"
        },
        {
          "Year": 1988,
          "Continent": "North America",
          "Female_Percentage": 0.32998324958123953,
          "Female Percentage": "33.0%"
        },
        {
          "Year": 1992,
          "Continent": "North America",
          "Female_Percentage": 0.3336653386454183,
          "Female Percentage": "33.4%"
        },
        {
          "Year": 1996,
          "Continent": "North America",
          "Female_Percentage": 0.3953257086026852,
          "Female Percentage": "39.5%"
        },
        {
          "Year": 2000,
          "Continent": "North America",
          "Female_Percentage": 0.4241469816272966,
          "Female Percentage": "42.4%"
        },
        {
          "Year": 2004,
          "Continent": "North America",
          "Female_Percentage": 0.4470720720720721,
          "Female Percentage": "44.7%"
        },
        {
          "Year": 2008,
          "Continent": "North America",
          "Female_Percentage": 0.4338074398249453,
          "Female Percentage": "43.4%"
        },
        {
          "Year": 2012,
          "Continent": "North America",
          "Female_Percentage": 0.4791666666666667,
          "Female Percentage": "47.9%"
        },
        {
          "Year": 2016,
          "Continent": "North America",
          "Female_Percentage": 0.4955947136563877,
          "Female Percentage": "49.6%"
        },
        {
          "Year": 1896,
          "Continent": "Oceania",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1900,
          "Continent": "Oceania",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1904,
          "Continent": "Oceania",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1906,
          "Continent": "Oceania",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1908,
          "Continent": "Oceania",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1912,
          "Continent": "Oceania",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1920,
          "Continent": "Oceania",
          "Female_Percentage": 0.14285714285714285,
          "Female Percentage": "14.3%"
        },
        {
          "Year": 1924,
          "Continent": "Oceania",
          "Female_Percentage": 0.045454545454545456,
          "Female Percentage": "4.5%"
        },
        {
          "Year": 1928,
          "Continent": "Oceania",
          "Female_Percentage": 0.2857142857142857,
          "Female Percentage": "28.6%"
        },
        {
          "Year": 1932,
          "Continent": "Oceania",
          "Female_Percentage": 0.12244897959183673,
          "Female Percentage": "12.2%"
        },
        {
          "Year": 1936,
          "Continent": "Oceania",
          "Female_Percentage": 0.125,
          "Female Percentage": "12.5%"
        },
        {
          "Year": 1948,
          "Continent": "Oceania",
          "Female_Percentage": 0.17117117117117114,
          "Female Percentage": "17.1%"
        },
        {
          "Year": 1952,
          "Continent": "Oceania",
          "Female_Percentage": 0.1375,
          "Female Percentage": "13.8%"
        },
        {
          "Year": 1956,
          "Continent": "Oceania",
          "Female_Percentage": 0.1729957805907173,
          "Female Percentage": "17.3%"
        },
        {
          "Year": 1960,
          "Continent": "Oceania",
          "Female_Percentage": 0.18787878787878787,
          "Female Percentage": "18.8%"
        },
        {
          "Year": 1964,
          "Continent": "Oceania",
          "Female_Percentage": 0.2375,
          "Female Percentage": "23.8%"
        },
        {
          "Year": 1968,
          "Continent": "Oceania",
          "Female_Percentage": 0.25862068965517243,
          "Female Percentage": "25.9%"
        },
        {
          "Year": 1972,
          "Continent": "Oceania",
          "Female_Percentage": 0.2356020942408377,
          "Female Percentage": "23.6%"
        },
        {
          "Year": 1976,
          "Continent": "Oceania",
          "Female_Percentage": 0.2383419689119171,
          "Female Percentage": "23.8%"
        },
        {
          "Year": 1980,
          "Continent": "Oceania",
          "Female_Percentage": 0.29949238578680204,
          "Female Percentage": "29.9%"
        },
        {
          "Year": 1984,
          "Continent": "Oceania",
          "Female_Percentage": 0.2949640287769784,
          "Female Percentage": "29.5%"
        },
        {
          "Year": 1988,
          "Continent": "Oceania",
          "Female_Percentage": 0.2690972222222222,
          "Female Percentage": "26.9%"
        },
        {
          "Year": 1992,
          "Continent": "Oceania",
          "Female_Percentage": 0.3381712626995646,
          "Female Percentage": "33.8%"
        },
        {
          "Year": 1996,
          "Continent": "Oceania",
          "Female_Percentage": 0.3949801849405548,
          "Female Percentage": "39.5%"
        },
        {
          "Year": 2000,
          "Continent": "Oceania",
          "Female_Percentage": 0.4650934119960669,
          "Female Percentage": "46.5%"
        },
        {
          "Year": 2004,
          "Continent": "Oceania",
          "Female_Percentage": 0.4480286738351255,
          "Female Percentage": "44.8%"
        },
        {
          "Year": 2008,
          "Continent": "Oceania",
          "Female_Percentage": 0.4597839135654262,
          "Female Percentage": "46.0%"
        },
        {
          "Year": 2012,
          "Continent": "Oceania",
          "Female_Percentage": 0.4623115577889447,
          "Female Percentage": "46.2%"
        },
        {
          "Year": 2016,
          "Continent": "Oceania",
          "Female_Percentage": 0.4833141542002302,
          "Female Percentage": "48.3%"
        },
        {
          "Year": 1896,
          "Continent": "South America",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1900,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1904,
          "Continent": "South America",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1906,
          "Continent": "South America",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1908,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1912,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1920,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1924,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1928,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1932,
          "Continent": "South America",
          "Female_Percentage": 0.023809523809523808,
          "Female Percentage": "2.4%"
        },
        {
          "Year": 1936,
          "Continent": "South America",
          "Female_Percentage": 0.03205128205128205,
          "Female Percentage": "3.2%"
        },
        {
          "Year": 1948,
          "Continent": "South America",
          "Female_Percentage": 0.08225806451612902,
          "Female Percentage": "8.2%"
        },
        {
          "Year": 1952,
          "Continent": "South America",
          "Female_Percentage": 0.07068607068607069,
          "Female Percentage": "7.1%"
        },
        {
          "Year": 1956,
          "Continent": "South America",
          "Female_Percentage": 0.021428571428571432,
          "Female Percentage": "2.1%"
        },
        {
          "Year": 1960,
          "Continent": "South America",
          "Female_Percentage": 0.03523035230352303,
          "Female Percentage": "3.5%"
        },
        {
          "Year": 1964,
          "Continent": "South America",
          "Female_Percentage": 0.04132231404958678,
          "Female Percentage": "4.1%"
        },
        {
          "Year": 1968,
          "Continent": "South America",
          "Female_Percentage": 0.15560165975103735,
          "Female Percentage": "15.6%"
        },
        {
          "Year": 1972,
          "Continent": "South America",
          "Female_Percentage": 0.117096018735363,
          "Female Percentage": "11.7%"
        },
        {
          "Year": 1976,
          "Continent": "South America",
          "Female_Percentage": 0.2050561797752809,
          "Female Percentage": "20.5%"
        },
        {
          "Year": 1980,
          "Continent": "South America",
          "Female_Percentage": 0.14788732394366194,
          "Female Percentage": "14.8%"
        },
        {
          "Year": 1984,
          "Continent": "South America",
          "Female_Percentage": 0.13333333333333333,
          "Female Percentage": "13.3%"
        },
        {
          "Year": 1988,
          "Continent": "South America",
          "Female_Percentage": 0.2332155477031802,
          "Female Percentage": "23.3%"
        },
        {
          "Year": 1992,
          "Continent": "South America",
          "Female_Percentage": 0.2249560632688928,
          "Female Percentage": "22.5%"
        },
        {
          "Year": 1996,
          "Continent": "South America",
          "Female_Percentage": 0.2697095435684647,
          "Female Percentage": "27.0%"
        },
        {
          "Year": 2000,
          "Continent": "South America",
          "Female_Percentage": 0.366306027820711,
          "Female Percentage": "36.6%"
        },
        {
          "Year": 2004,
          "Continent": "South America",
          "Female_Percentage": 0.39811066126855604,
          "Female Percentage": "39.8%"
        },
        {
          "Year": 2008,
          "Continent": "South America",
          "Female_Percentage": 0.4339152119700748,
          "Female Percentage": "43.4%"
        },
        {
          "Year": 2012,
          "Continent": "South America",
          "Female_Percentage": 0.4207920792079208,
          "Female Percentage": "42.1%"
        },
        {
          "Year": 2016,
          "Continent": "South America",
          "Female_Percentage": 0.4156674660271783,
          "Female Percentage": "41.6%"
        }
      ]
    },
    {
      "name": "data_0",
      "source": "data-c9cd4958aa454941ccfb344427499b56",
      "transform": [
        {"type": "formula", "expr": "toNumber(datum[\"Year\"])", "as": "Year"}
      ]
    }
  ],
  "signals": [
    {
      "name": "unit",
      "value": {},
      "on": [
        {"events": "mousemove", "update": "isTuple(group()) ? group() : unit"}
      ]
    },
    {
      "name": "selector010",
      "update": "vlSelectionResolve(\"selector010_store\", \"union\")"
    },
    {
      "name": "selector010_Year",
      "on": [
        {
          "events": {"signal": "selector010_translate_delta"},
          "update": "panLinear(selector010_translate_anchor.extent_x, -selector010_translate_delta.x / width)"
        },
        {
          "events": {"signal": "selector010_zoom_delta"},
          "update": "zoomLinear(domain(\"x\"), selector010_zoom_anchor.x, selector010_zoom_delta)"
        },
        {"events": [{"source": "scope", "type": "dblclick"}], "update": "null"}
      ]
    },
    {
      "name": "selector010_Female_Percentage",
      "on": [
        {
          "events": {"signal": "selector010_translate_delta"},
          "update": "panLinear(selector010_translate_anchor.extent_y, selector010_translate_delta.y / height)"
        },
        {
          "events": {"signal": "selector010_zoom_delta"},
          "update": "zoomLinear(domain(\"y\"), selector010_zoom_anchor.y, selector010_zoom_delta)"
        },
        {"events": [{"source": "scope", "type": "dblclick"}], "update": "null"}
      ]
    },
    {
      "name": "selector010_tuple",
      "on": [
        {
          "events": [
            {"signal": "selector010_Year || selector010_Female_Percentage"}
          ],
          "update": "selector010_Year && selector010_Female_Percentage ? {unit: \"\", fields: selector010_tuple_fields, values: [selector010_Year,selector010_Female_Percentage]} : null"
        }
      ]
    },
    {
      "name": "selector010_tuple_fields",
      "value": [
        {"field": "Year", "channel": "x", "type": "R"},
        {"field": "Female_Percentage", "channel": "y", "type": "R"}
      ]
    },
    {
      "name": "selector010_translate_anchor",
      "value": {},
      "on": [
        {
          "events": [{"source": "scope", "type": "mousedown"}],
          "update": "{x: x(unit), y: y(unit), extent_x: domain(\"x\"), extent_y: domain(\"y\")}"
        }
      ]
    },
    {
      "name": "selector010_translate_delta",
      "value": {},
      "on": [
        {
          "events": [
            {
              "source": "window",
              "type": "mousemove",
              "consume": true,
              "between": [
                {"source": "scope", "type": "mousedown"},
                {"source": "window", "type": "mouseup"}
              ]
            }
          ],
          "update": "{x: selector010_translate_anchor.x - x(unit), y: selector010_translate_anchor.y - y(unit)}"
        }
      ]
    },
    {
      "name": "selector010_zoom_anchor",
      "on": [
        {
          "events": [{"source": "scope", "type": "wheel", "consume": true}],
          "update": "{x: invert(\"x\", x(unit)), y: invert(\"y\", y(unit))}"
        }
      ]
    },
    {
      "name": "selector010_zoom_delta",
      "on": [
        {
          "events": [{"source": "scope", "type": "wheel", "consume": true}],
          "force": true,
          "update": "pow(1.001, event.deltaY * pow(16, event.deltaMode))"
        }
      ]
    },
    {
      "name": "selector010_modify",
      "on": [
        {
          "events": {"signal": "selector010_tuple"},
          "update": "modify(\"selector010_store\", selector010_tuple, true)"
        }
      ]
    }
  ],
  "marks": [
    {
      "name": "pathgroup",
      "type": "group",
      "from": {
        "facet": {
          "name": "faceted_path_main",
          "data": "data_0",
          "groupby": ["Continent"]
        }
      },
      "encode": {
        "update": {
          "width": {"field": {"group": "width"}},
          "height": {"field": {"group": "height"}}
        }
      },
      "marks": [
        {
          "name": "marks",
          "type": "line",
          "clip": true,
          "style": ["line"],
          "sort": {"field": "datum[\"Year\"]"},
          "interactive": true,
          "from": {"data": "faceted_path_main"},
          "encode": {
            "update": {
              "stroke": {"scale": "color", "field": "Continent"},
              "tooltip": {
                "signal": "{\"Year\": format(datum[\"Year\"], \"\"), \"Continent\": isValid(datum[\"Continent\"]) ? datum[\"Continent\"] : \"\"+datum[\"Continent\"], \"Female Percentage\": isValid(datum[\"Female Percentage\"]) ? datum[\"Female Percentage\"] : \"\"+datum[\"Female Percentage\"]}"
              },
              "description": {
                "signal": "\"Continent\" + \": \" + (isValid(datum[\"Continent\"]) ? datum[\"Continent\"] : \"\"+datum[\"Continent\"]) + \"; \" + \"Year\" + \": \" + (format(datum[\"Year\"], \"\")) + \"; \" + \"Female Percentage\" + \": \" + (format(datum[\"Female_Percentage\"], \"\"))"
              },
              "x": {"scale": "x", "field": "Year"},
              "y": {"scale": "y", "field": "Female_Percentage"},
              "strokeWidth": {"value": 4},
              "defined": {
                "signal": "isValid(datum[\"Year\"]) && isFinite(+datum[\"Year\"]) && isValid(datum[\"Female_Percentage\"]) && isFinite(+datum[\"Female_Percentage\"])"
              }
            }
          }
        }
      ]
    }
  ],
  "scales": [
    {
      "name": "x",
      "type": "linear",
      "domain": {"data": "data_0", "field": "Year"},
      "domainRaw": {"signal": "selector010[\"Year\"]"},
      "range": [0, {"signal": "width"}],
      "nice": true,
      "zero": false
    },
    {
      "name": "y",
      "type": "linear",
      "domain": {"data": "data_0", "field": "Female_Percentage"},
      "domainRaw": {"signal": "selector010[\"Female_Percentage\"]"},
      "range": [{"signal": "height"}, 0],
      "nice": true,
      "zero": true
    },
    {
      "name": "color",
      "type": "ordinal",
      "domain": {"data": "data_0", "field": "Continent", "sort": true},
      "range": "category"
    }
  ],
  "axes": [
    {
      "scale": "x",
      "orient": "bottom",
      "gridScale": "y",
      "grid": true,
      "tickCount": {"signal": "ceil(width/40)"},
      "domain": false,
      "labels": false,
      "aria": false,
      "maxExtent": 0,
      "minExtent": 0,
      "ticks": false,
      "zindex": 0
    },
    {
      "scale": "y",
      "orient": "left",
      "gridScale": "x",
      "grid": true,
      "tickCount": {"signal": "ceil(height/40)"},
      "domain": false,
      "labels": false,
      "aria": false,
      "maxExtent": 0,
      "minExtent": 0,
      "ticks": false,
      "zindex": 0
    },
    {
      "scale": "x",
      "orient": "bottom",
      "grid": false,
      "title": "Year",
      "labelFlush": true,
      "labelOverlap": true,
      "tickCount": {"signal": "ceil(width/40)"},
      "zindex": 0
    },
    {
      "scale": "y",
      "orient": "left",
      "grid": false,
      "title": "Female Percentage",
      "labelOverlap": true,
      "tickCount": {"signal": "ceil(height/40)"},
      "zindex": 0
    }
  ],
  "legends": [
    {"stroke": "color", "symbolType": "stroke", "title": "Continent"}
  ],
  "config": {
    "legend": {
      "cornerRadius": 10,
      "fillColor": "#EEEEEE",
      "labelFontSize": 14,
      "padding": 10,
      "strokeColor": "gray"
    },
    "style": {"group-title": {"fontSize": 18}},
    "axis": {"labelFontSize": 12, "titleFontSize": 14}
  }
};

vegaEmbed('#figure27', figure27);
</script>

<script type="text/javascript">
var figure28_2 = {
  "$schema": "https://vega.github.io/schema/vega/v5.json",
  "background": "white",
  "padding": 5,
  "title": {
    "anchor": "middle",
    "text": "Changes in female athletes participation in Summer Olympics"
  },
  "data": [
    {"name": "selector069_store"},
    {
      "name": "data-c9cd4958aa454941ccfb344427499b56",
      "values": [
        {
          "Year": 1896,
          "Continent": "Global",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1900,
          "Continent": "Global",
          "Female_Percentage": 0.016045548654244308,
          "Female Percentage": "1.6%"
        },
        {
          "Year": 1904,
          "Continent": "Global",
          "Female_Percentage": 0.012307692307692308,
          "Female Percentage": "1.2%"
        },
        {
          "Year": 1906,
          "Continent": "Global",
          "Female_Percentage": 0.006489675516224189,
          "Female Percentage": "0.6%"
        },
        {
          "Year": 1908,
          "Continent": "Global",
          "Female_Percentage": 0.015568068896985756,
          "Female Percentage": "1.6%"
        },
        {
          "Year": 1912,
          "Continent": "Global",
          "Female_Percentage": 0.020242914979757085,
          "Female Percentage": "2.0%"
        },
        {
          "Year": 1920,
          "Continent": "Global",
          "Female_Percentage": 0.03247863247863248,
          "Female Percentage": "3.2%"
        },
        {
          "Year": 1924,
          "Continent": "Global",
          "Female_Percentage": 0.04917363803305448,
          "Female Percentage": "4.9%"
        },
        {
          "Year": 1928,
          "Continent": "Global",
          "Female_Percentage": 0.08397582829756199,
          "Female Percentage": "8.4%"
        },
        {
          "Year": 1932,
          "Continent": "Global",
          "Female_Percentage": 0.11859193438140808,
          "Female Percentage": "11.9%"
        },
        {
          "Year": 1936,
          "Continent": "Global",
          "Female_Percentage": 0.07177974434611603,
          "Female Percentage": "7.2%"
        },
        {
          "Year": 1948,
          "Continent": "Global",
          "Female_Percentage": 0.0974740932642487,
          "Female Percentage": "9.7%"
        },
        {
          "Year": 1952,
          "Continent": "Global",
          "Female_Percentage": 0.17301414581066374,
          "Female Percentage": "17.3%"
        },
        {
          "Year": 1956,
          "Continent": "Global",
          "Female_Percentage": 0.1704136690647482,
          "Female Percentage": "17.0%"
        },
        {
          "Year": 1960,
          "Continent": "Global",
          "Female_Percentage": 0.1761111111111111,
          "Female Percentage": "17.6%"
        },
        {
          "Year": 1964,
          "Continent": "Global",
          "Female_Percentage": 0.17183667580435724,
          "Female Percentage": "17.2%"
        },
        {
          "Year": 1968,
          "Continent": "Global",
          "Female_Percentage": 0.19755020652328728,
          "Female Percentage": "19.8%"
        },
        {
          "Year": 1972,
          "Continent": "Global",
          "Female_Percentage": 0.2010383965225791,
          "Female Percentage": "20.1%"
        },
        {
          "Year": 1976,
          "Continent": "Global",
          "Female_Percentage": 0.2333720592506535,
          "Female Percentage": "23.3%"
        },
        {
          "Year": 1980,
          "Continent": "Global",
          "Female_Percentage": 0.22398271516024487,
          "Female Percentage": "22.4%"
        },
        {
          "Year": 1984,
          "Continent": "Global",
          "Female_Percentage": 0.25244707489187346,
          "Female Percentage": "25.2%"
        },
        {
          "Year": 1988,
          "Continent": "Global",
          "Female_Percentage": 0.2830937035200793,
          "Female Percentage": "28.3%"
        },
        {
          "Year": 1992,
          "Continent": "Global",
          "Female_Percentage": 0.3129472457979697,
          "Female Percentage": "31.3%"
        },
        {
          "Year": 1996,
          "Continent": "Global",
          "Female_Percentage": 0.36325520654340493,
          "Female Percentage": "36.3%"
        },
        {
          "Year": 2000,
          "Continent": "Global",
          "Female_Percentage": 0.3939145299145299,
          "Female Percentage": "39.4%"
        },
        {
          "Year": 2004,
          "Continent": "Global",
          "Female_Percentage": 0.4132602893664841,
          "Female Percentage": "41.3%"
        },
        {
          "Year": 2008,
          "Continent": "Global",
          "Female_Percentage": 0.4284037558685446,
          "Female Percentage": "42.8%"
        },
        {
          "Year": 2012,
          "Continent": "Global",
          "Female_Percentage": 0.4500399100210435,
          "Female Percentage": "45.0%"
        },
        {
          "Year": 2016,
          "Continent": "Global",
          "Female_Percentage": 0.4535101729046594,
          "Female Percentage": "45.4%"
        },
        {
          "Year": 1896,
          "Continent": "Africa",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1900,
          "Continent": "Africa",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1904,
          "Continent": "Africa",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1906,
          "Continent": "Africa",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1908,
          "Continent": "Africa",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1912,
          "Continent": "Africa",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1920,
          "Continent": "Africa",
          "Female_Percentage": 0.01680672268907563,
          "Female Percentage": "1.7%"
        },
        {
          "Year": 1924,
          "Continent": "Africa",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1928,
          "Continent": "Africa",
          "Female_Percentage": 0.1411764705882353,
          "Female Percentage": "14.1%"
        },
        {
          "Year": 1932,
          "Continent": "Africa",
          "Female_Percentage": 0.25,
          "Female Percentage": "25.0%"
        },
        {
          "Year": 1936,
          "Continent": "Africa",
          "Female_Percentage": 0.1,
          "Female Percentage": "10.0%"
        },
        {
          "Year": 1948,
          "Continent": "Africa",
          "Female_Percentage": 0.009569377990430622,
          "Female Percentage": "1.0%"
        },
        {
          "Year": 1952,
          "Continent": "Africa",
          "Female_Percentage": 0.02735562310030395,
          "Female Percentage": "2.7%"
        },
        {
          "Year": 1956,
          "Continent": "Africa",
          "Female_Percentage": 0.0748663101604278,
          "Female Percentage": "7.5%"
        },
        {
          "Year": 1960,
          "Continent": "Africa",
          "Female_Percentage": 0.04456824512534819,
          "Female Percentage": "4.5%"
        },
        {
          "Year": 1964,
          "Continent": "Africa",
          "Female_Percentage": 0.045454545454545456,
          "Female Percentage": "4.5%"
        },
        {
          "Year": 1968,
          "Continent": "Africa",
          "Female_Percentage": 0.039886039886039885,
          "Female Percentage": "4.0%"
        },
        {
          "Year": 1972,
          "Continent": "Africa",
          "Female_Percentage": 0.056985294117647065,
          "Female Percentage": "5.7%"
        },
        {
          "Year": 1976,
          "Continent": "Africa",
          "Female_Percentage": 0.0707070707070707,
          "Female Percentage": "7.1%"
        },
        {
          "Year": 1980,
          "Continent": "Africa",
          "Female_Percentage": 0.1524590163934426,
          "Female Percentage": "15.2%"
        },
        {
          "Year": 1984,
          "Continent": "Africa",
          "Female_Percentage": 0.09419354838709676,
          "Female Percentage": "9.4%"
        },
        {
          "Year": 1988,
          "Continent": "Africa",
          "Female_Percentage": 0.13974799541809851,
          "Female Percentage": "14.0%"
        },
        {
          "Year": 1992,
          "Continent": "Africa",
          "Female_Percentage": 0.22341568206229864,
          "Female Percentage": "22.3%"
        },
        {
          "Year": 1996,
          "Continent": "Africa",
          "Female_Percentage": 0.2462077012835473,
          "Female Percentage": "24.6%"
        },
        {
          "Year": 2000,
          "Continent": "Africa",
          "Female_Percentage": 0.3296370967741936,
          "Female Percentage": "33.0%"
        },
        {
          "Year": 2004,
          "Continent": "Africa",
          "Female_Percentage": 0.33407572383073497,
          "Female Percentage": "33.4%"
        },
        {
          "Year": 2008,
          "Continent": "Africa",
          "Female_Percentage": 0.3874734607218684,
          "Female Percentage": "38.7%"
        },
        {
          "Year": 2012,
          "Continent": "Africa",
          "Female_Percentage": 0.399581589958159,
          "Female Percentage": "40.0%"
        },
        {
          "Year": 2016,
          "Continent": "Africa",
          "Female_Percentage": 0.3836772983114447,
          "Female Percentage": "38.4%"
        },
        {
          "Year": 1896,
          "Continent": "Asia",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1900,
          "Continent": "Asia",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1904,
          "Continent": "Asia",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1906,
          "Continent": "Asia",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1908,
          "Continent": "Asia",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1912,
          "Continent": "Asia",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1920,
          "Continent": "Asia",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1924,
          "Continent": "Asia",
          "Female_Percentage": 0.033707865168539325,
          "Female Percentage": "3.4%"
        },
        {
          "Year": 1928,
          "Continent": "Asia",
          "Female_Percentage": 0.015873015873015872,
          "Female Percentage": "1.6%"
        },
        {
          "Year": 1932,
          "Continent": "Asia",
          "Female_Percentage": 0.11203319502074688,
          "Female Percentage": "11.2%"
        },
        {
          "Year": 1936,
          "Continent": "Asia",
          "Female_Percentage": 0.057620817843866176,
          "Female Percentage": "5.8%"
        },
        {
          "Year": 1948,
          "Continent": "Asia",
          "Female_Percentage": 0.0069124423963133645,
          "Female Percentage": "0.7%"
        },
        {
          "Year": 1952,
          "Continent": "Asia",
          "Female_Percentage": 0.065439672801636,
          "Female Percentage": "6.5%"
        },
        {
          "Year": 1956,
          "Continent": "Asia",
          "Female_Percentage": 0.1060126582278481,
          "Female Percentage": "10.6%"
        },
        {
          "Year": 1960,
          "Continent": "Asia",
          "Female_Percentage": 0.129366106080207,
          "Female Percentage": "12.9%"
        },
        {
          "Year": 1964,
          "Continent": "Asia",
          "Female_Percentage": 0.14587593728698026,
          "Female Percentage": "14.6%"
        },
        {
          "Year": 1968,
          "Continent": "Asia",
          "Female_Percentage": 0.17119244391971666,
          "Female Percentage": "17.1%"
        },
        {
          "Year": 1972,
          "Continent": "Asia",
          "Female_Percentage": 0.14781746031746032,
          "Female Percentage": "14.8%"
        },
        {
          "Year": 1976,
          "Continent": "Asia",
          "Female_Percentage": 0.16761041902604756,
          "Female Percentage": "16.8%"
        },
        {
          "Year": 1980,
          "Continent": "Asia",
          "Female_Percentage": 0.1494661921708185,
          "Female Percentage": "14.9%"
        },
        {
          "Year": 1984,
          "Continent": "Asia",
          "Female_Percentage": 0.2409855769230769,
          "Female Percentage": "24.1%"
        },
        {
          "Year": 1988,
          "Continent": "Asia",
          "Female_Percentage": 0.3037466547725245,
          "Female Percentage": "30.4%"
        },
        {
          "Year": 1992,
          "Continent": "Asia",
          "Female_Percentage": 0.31186440677966104,
          "Female Percentage": "31.2%"
        },
        {
          "Year": 1996,
          "Continent": "Asia",
          "Female_Percentage": 0.3821571238348868,
          "Female Percentage": "38.2%"
        },
        {
          "Year": 2000,
          "Continent": "Asia",
          "Female_Percentage": 0.39642620780939775,
          "Female Percentage": "39.6%"
        },
        {
          "Year": 2004,
          "Continent": "Asia",
          "Female_Percentage": 0.4359058207979071,
          "Female Percentage": "43.6%"
        },
        {
          "Year": 2008,
          "Continent": "Asia",
          "Female_Percentage": 0.43423423423423424,
          "Female Percentage": "43.4%"
        },
        {
          "Year": 2012,
          "Continent": "Asia",
          "Female_Percentage": 0.4599396580623533,
          "Female Percentage": "46.0%"
        },
        {
          "Year": 2016,
          "Continent": "Asia",
          "Female_Percentage": 0.4653897849462366,
          "Female Percentage": "46.5%"
        },
        {
          "Year": 1896,
          "Continent": "Europe",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1900,
          "Continent": "Europe",
          "Female_Percentage": 0.012528473804100227,
          "Female Percentage": "1.3%"
        },
        {
          "Year": 1904,
          "Continent": "Europe",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1906,
          "Continent": "Europe",
          "Female_Percentage": 0.006905210295040804,
          "Female Percentage": "0.7%"
        },
        {
          "Year": 1908,
          "Continent": "Europe",
          "Female_Percentage": 0.01800076599004213,
          "Female Percentage": "1.8%"
        },
        {
          "Year": 1912,
          "Continent": "Europe",
          "Female_Percentage": 0.024897480960749854,
          "Female Percentage": "2.5%"
        },
        {
          "Year": 1920,
          "Continent": "Europe",
          "Female_Percentage": 0.03142943487458446,
          "Female Percentage": "3.1%"
        },
        {
          "Year": 1924,
          "Continent": "Europe",
          "Female_Percentage": 0.05149330587023687,
          "Female Percentage": "5.1%"
        },
        {
          "Year": 1928,
          "Continent": "Europe",
          "Female_Percentage": 0.0821664464993395,
          "Female Percentage": "8.2%"
        },
        {
          "Year": 1932,
          "Continent": "Europe",
          "Female_Percentage": 0.10588235294117647,
          "Female Percentage": "10.6%"
        },
        {
          "Year": 1936,
          "Continent": "Europe",
          "Female_Percentage": 0.06700091157702825,
          "Female Percentage": "6.7%"
        },
        {
          "Year": 1948,
          "Continent": "Europe",
          "Female_Percentage": 0.1073929961089494,
          "Female Percentage": "10.7%"
        },
        {
          "Year": 1952,
          "Continent": "Europe",
          "Female_Percentage": 0.20599325262949,
          "Female Percentage": "20.6%"
        },
        {
          "Year": 1956,
          "Continent": "Europe",
          "Female_Percentage": 0.20808451998162608,
          "Female Percentage": "20.8%"
        },
        {
          "Year": 1960,
          "Continent": "Europe",
          "Female_Percentage": 0.19808861859252824,
          "Female Percentage": "19.8%"
        },
        {
          "Year": 1964,
          "Continent": "Europe",
          "Female_Percentage": 0.19008009858287125,
          "Female Percentage": "19.0%"
        },
        {
          "Year": 1968,
          "Continent": "Europe",
          "Female_Percentage": 0.20454545454545456,
          "Female Percentage": "20.5%"
        },
        {
          "Year": 1972,
          "Continent": "Europe",
          "Female_Percentage": 0.22300968580203165,
          "Female Percentage": "22.3%"
        },
        {
          "Year": 1976,
          "Continent": "Europe",
          "Female_Percentage": 0.2362555720653789,
          "Female Percentage": "23.6%"
        },
        {
          "Year": 1980,
          "Continent": "Europe",
          "Female_Percentage": 0.257801108194809,
          "Female Percentage": "25.8%"
        },
        {
          "Year": 1984,
          "Continent": "Europe",
          "Female_Percentage": 0.2688271604938272,
          "Female Percentage": "26.9%"
        },
        {
          "Year": 1988,
          "Continent": "Europe",
          "Female_Percentage": 0.29081000743126084,
          "Female Percentage": "29.1%"
        },
        {
          "Year": 1992,
          "Continent": "Europe",
          "Female_Percentage": 0.3262682418346073,
          "Female Percentage": "32.6%"
        },
        {
          "Year": 1996,
          "Continent": "Europe",
          "Female_Percentage": 0.3664026677782409,
          "Female Percentage": "36.6%"
        },
        {
          "Year": 2000,
          "Continent": "Europe",
          "Female_Percentage": 0.38596989491621697,
          "Female Percentage": "38.6%"
        },
        {
          "Year": 2004,
          "Continent": "Europe",
          "Female_Percentage": 0.4022806004618938,
          "Female Percentage": "40.2%"
        },
        {
          "Year": 2008,
          "Continent": "Europe",
          "Female_Percentage": 0.4252481849162839,
          "Female Percentage": "42.5%"
        },
        {
          "Year": 2012,
          "Continent": "Europe",
          "Female_Percentage": 0.4477747502270663,
          "Female Percentage": "44.8%"
        },
        {
          "Year": 2016,
          "Continent": "Europe",
          "Female_Percentage": 0.4510353417406197,
          "Female Percentage": "45.1%"
        },
        {
          "Year": 1896,
          "Continent": "North America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1900,
          "Continent": "North America",
          "Female_Percentage": 0.05960264900662252,
          "Female Percentage": "6.0%"
        },
        {
          "Year": 1904,
          "Continent": "North America",
          "Female_Percentage": 0.013605442176870748,
          "Female Percentage": "1.4%"
        },
        {
          "Year": 1906,
          "Continent": "North America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1908,
          "Continent": "North America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1912,
          "Continent": "North America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1920,
          "Continent": "North America",
          "Female_Percentage": 0.03942652329749104,
          "Female Percentage": "3.9%"
        },
        {
          "Year": 1924,
          "Continent": "North America",
          "Female_Percentage": 0.05843071786310518,
          "Female Percentage": "5.8%"
        },
        {
          "Year": 1928,
          "Continent": "North America",
          "Female_Percentage": 0.11,
          "Female Percentage": "11.0%"
        },
        {
          "Year": 1932,
          "Continent": "North America",
          "Female_Percentage": 0.14641148325358852,
          "Female Percentage": "14.6%"
        },
        {
          "Year": 1936,
          "Continent": "North America",
          "Female_Percentage": 0.1221264367816092,
          "Female Percentage": "12.2%"
        },
        {
          "Year": 1948,
          "Continent": "North America",
          "Female_Percentage": 0.11932418162618795,
          "Female Percentage": "11.9%"
        },
        {
          "Year": 1952,
          "Continent": "North America",
          "Female_Percentage": 0.16042154566744732,
          "Female Percentage": "16.0%"
        },
        {
          "Year": 1956,
          "Continent": "North America",
          "Female_Percentage": 0.19484240687679086,
          "Female Percentage": "19.5%"
        },
        {
          "Year": 1960,
          "Continent": "North America",
          "Female_Percentage": 0.21568627450980396,
          "Female Percentage": "21.6%"
        },
        {
          "Year": 1964,
          "Continent": "North America",
          "Female_Percentage": 0.2101661779081134,
          "Female Percentage": "21.0%"
        },
        {
          "Year": 1968,
          "Continent": "North America",
          "Female_Percentage": 0.2272957889396245,
          "Female Percentage": "22.7%"
        },
        {
          "Year": 1972,
          "Continent": "North America",
          "Female_Percentage": 0.23755924170616116,
          "Female Percentage": "23.8%"
        },
        {
          "Year": 1976,
          "Continent": "North America",
          "Female_Percentage": 0.27378964941569284,
          "Female Percentage": "27.4%"
        },
        {
          "Year": 1980,
          "Continent": "North America",
          "Female_Percentage": 0.17372881355932204,
          "Female Percentage": "17.4%"
        },
        {
          "Year": 1984,
          "Continent": "North America",
          "Female_Percentage": 0.3223987698616094,
          "Female Percentage": "32.2%"
        },
        {
          "Year": 1988,
          "Continent": "North America",
          "Female_Percentage": 0.32998324958123953,
          "Female Percentage": "33.0%"
        },
        {
          "Year": 1992,
          "Continent": "North America",
          "Female_Percentage": 0.3336653386454183,
          "Female Percentage": "33.4%"
        },
        {
          "Year": 1996,
          "Continent": "North America",
          "Female_Percentage": 0.3953257086026852,
          "Female Percentage": "39.5%"
        },
        {
          "Year": 2000,
          "Continent": "North America",
          "Female_Percentage": 0.4241469816272966,
          "Female Percentage": "42.4%"
        },
        {
          "Year": 2004,
          "Continent": "North America",
          "Female_Percentage": 0.4470720720720721,
          "Female Percentage": "44.7%"
        },
        {
          "Year": 2008,
          "Continent": "North America",
          "Female_Percentage": 0.4338074398249453,
          "Female Percentage": "43.4%"
        },
        {
          "Year": 2012,
          "Continent": "North America",
          "Female_Percentage": 0.4791666666666667,
          "Female Percentage": "47.9%"
        },
        {
          "Year": 2016,
          "Continent": "North America",
          "Female_Percentage": 0.4955947136563877,
          "Female Percentage": "49.6%"
        },
        {
          "Year": 1896,
          "Continent": "Oceania",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1900,
          "Continent": "Oceania",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1904,
          "Continent": "Oceania",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1906,
          "Continent": "Oceania",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1908,
          "Continent": "Oceania",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1912,
          "Continent": "Oceania",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1920,
          "Continent": "Oceania",
          "Female_Percentage": 0.14285714285714285,
          "Female Percentage": "14.3%"
        },
        {
          "Year": 1924,
          "Continent": "Oceania",
          "Female_Percentage": 0.045454545454545456,
          "Female Percentage": "4.5%"
        },
        {
          "Year": 1928,
          "Continent": "Oceania",
          "Female_Percentage": 0.2857142857142857,
          "Female Percentage": "28.6%"
        },
        {
          "Year": 1932,
          "Continent": "Oceania",
          "Female_Percentage": 0.12244897959183673,
          "Female Percentage": "12.2%"
        },
        {
          "Year": 1936,
          "Continent": "Oceania",
          "Female_Percentage": 0.125,
          "Female Percentage": "12.5%"
        },
        {
          "Year": 1948,
          "Continent": "Oceania",
          "Female_Percentage": 0.17117117117117114,
          "Female Percentage": "17.1%"
        },
        {
          "Year": 1952,
          "Continent": "Oceania",
          "Female_Percentage": 0.1375,
          "Female Percentage": "13.8%"
        },
        {
          "Year": 1956,
          "Continent": "Oceania",
          "Female_Percentage": 0.1729957805907173,
          "Female Percentage": "17.3%"
        },
        {
          "Year": 1960,
          "Continent": "Oceania",
          "Female_Percentage": 0.18787878787878787,
          "Female Percentage": "18.8%"
        },
        {
          "Year": 1964,
          "Continent": "Oceania",
          "Female_Percentage": 0.2375,
          "Female Percentage": "23.8%"
        },
        {
          "Year": 1968,
          "Continent": "Oceania",
          "Female_Percentage": 0.25862068965517243,
          "Female Percentage": "25.9%"
        },
        {
          "Year": 1972,
          "Continent": "Oceania",
          "Female_Percentage": 0.2356020942408377,
          "Female Percentage": "23.6%"
        },
        {
          "Year": 1976,
          "Continent": "Oceania",
          "Female_Percentage": 0.2383419689119171,
          "Female Percentage": "23.8%"
        },
        {
          "Year": 1980,
          "Continent": "Oceania",
          "Female_Percentage": 0.29949238578680204,
          "Female Percentage": "29.9%"
        },
        {
          "Year": 1984,
          "Continent": "Oceania",
          "Female_Percentage": 0.2949640287769784,
          "Female Percentage": "29.5%"
        },
        {
          "Year": 1988,
          "Continent": "Oceania",
          "Female_Percentage": 0.2690972222222222,
          "Female Percentage": "26.9%"
        },
        {
          "Year": 1992,
          "Continent": "Oceania",
          "Female_Percentage": 0.3381712626995646,
          "Female Percentage": "33.8%"
        },
        {
          "Year": 1996,
          "Continent": "Oceania",
          "Female_Percentage": 0.3949801849405548,
          "Female Percentage": "39.5%"
        },
        {
          "Year": 2000,
          "Continent": "Oceania",
          "Female_Percentage": 0.4650934119960669,
          "Female Percentage": "46.5%"
        },
        {
          "Year": 2004,
          "Continent": "Oceania",
          "Female_Percentage": 0.4480286738351255,
          "Female Percentage": "44.8%"
        },
        {
          "Year": 2008,
          "Continent": "Oceania",
          "Female_Percentage": 0.4597839135654262,
          "Female Percentage": "46.0%"
        },
        {
          "Year": 2012,
          "Continent": "Oceania",
          "Female_Percentage": 0.4623115577889447,
          "Female Percentage": "46.2%"
        },
        {
          "Year": 2016,
          "Continent": "Oceania",
          "Female_Percentage": 0.4833141542002302,
          "Female Percentage": "48.3%"
        },
        {
          "Year": 1896,
          "Continent": "South America",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1900,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1904,
          "Continent": "South America",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1906,
          "Continent": "South America",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1908,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1912,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1920,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1924,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1928,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1932,
          "Continent": "South America",
          "Female_Percentage": 0.023809523809523808,
          "Female Percentage": "2.4%"
        },
        {
          "Year": 1936,
          "Continent": "South America",
          "Female_Percentage": 0.03205128205128205,
          "Female Percentage": "3.2%"
        },
        {
          "Year": 1948,
          "Continent": "South America",
          "Female_Percentage": 0.08225806451612902,
          "Female Percentage": "8.2%"
        },
        {
          "Year": 1952,
          "Continent": "South America",
          "Female_Percentage": 0.07068607068607069,
          "Female Percentage": "7.1%"
        },
        {
          "Year": 1956,
          "Continent": "South America",
          "Female_Percentage": 0.021428571428571432,
          "Female Percentage": "2.1%"
        },
        {
          "Year": 1960,
          "Continent": "South America",
          "Female_Percentage": 0.03523035230352303,
          "Female Percentage": "3.5%"
        },
        {
          "Year": 1964,
          "Continent": "South America",
          "Female_Percentage": 0.04132231404958678,
          "Female Percentage": "4.1%"
        },
        {
          "Year": 1968,
          "Continent": "South America",
          "Female_Percentage": 0.15560165975103735,
          "Female Percentage": "15.6%"
        },
        {
          "Year": 1972,
          "Continent": "South America",
          "Female_Percentage": 0.117096018735363,
          "Female Percentage": "11.7%"
        },
        {
          "Year": 1976,
          "Continent": "South America",
          "Female_Percentage": 0.2050561797752809,
          "Female Percentage": "20.5%"
        },
        {
          "Year": 1980,
          "Continent": "South America",
          "Female_Percentage": 0.14788732394366194,
          "Female Percentage": "14.8%"
        },
        {
          "Year": 1984,
          "Continent": "South America",
          "Female_Percentage": 0.13333333333333333,
          "Female Percentage": "13.3%"
        },
        {
          "Year": 1988,
          "Continent": "South America",
          "Female_Percentage": 0.2332155477031802,
          "Female Percentage": "23.3%"
        },
        {
          "Year": 1992,
          "Continent": "South America",
          "Female_Percentage": 0.2249560632688928,
          "Female Percentage": "22.5%"
        },
        {
          "Year": 1996,
          "Continent": "South America",
          "Female_Percentage": 0.2697095435684647,
          "Female Percentage": "27.0%"
        },
        {
          "Year": 2000,
          "Continent": "South America",
          "Female_Percentage": 0.366306027820711,
          "Female Percentage": "36.6%"
        },
        {
          "Year": 2004,
          "Continent": "South America",
          "Female_Percentage": 0.39811066126855604,
          "Female Percentage": "39.8%"
        },
        {
          "Year": 2008,
          "Continent": "South America",
          "Female_Percentage": 0.4339152119700748,
          "Female Percentage": "43.4%"
        },
        {
          "Year": 2012,
          "Continent": "South America",
          "Female_Percentage": 0.4207920792079208,
          "Female Percentage": "42.1%"
        },
        {
          "Year": 2016,
          "Continent": "South America",
          "Female_Percentage": 0.4156674660271783,
          "Female Percentage": "41.6%"
        }
      ]
    },
    {
      "name": "data_0",
      "source": "data-c9cd4958aa454941ccfb344427499b56",
      "transform": [
        {"type": "formula", "expr": "toNumber(datum[\"Year\"])", "as": "Year"}
      ]
    },
    {
      "name": "facet_domain",
      "source": "data_0",
      "transform": [{"type": "aggregate", "groupby": ["Continent"]}]
    },
    {
      "name": "facet_domain_row",
      "transform": [
        {
          "type": "sequence",
          "start": 0,
          "stop": {"signal": "ceil(length(data(\"facet_domain\")) / 3)"}
        }
      ]
    },
    {
      "name": "facet_domain_column",
      "transform": [
        {
          "type": "sequence",
          "start": 0,
          "stop": {"signal": "min(length(data(\"facet_domain\")), 3)"}
        }
      ]
    }
  ],
  "signals": [
    {"name": "child_width", "value": 200},
    {"name": "child_height", "value": 200},
    {
      "name": "unit",
      "value": {},
      "on": [
        {"events": "mousemove", "update": "isTuple(group()) ? group() : unit"}
      ]
    },
    {
      "name": "selector069",
      "update": "{\"Year\": selector069_Year, \"Female_Percentage\": selector069_Female_Percentage}"
    },
    {"name": "selector069_Year"},
    {"name": "selector069_Female_Percentage"}
  ],
  "layout": {"padding": 20, "bounds": "full", "align": "all", "columns": 3},
  "marks": [
    {
      "name": "facet-title",
      "type": "group",
      "role": "column-title",
      "title": {"text": "Continent", "style": "guide-title", "offset": 10}
    },
    {
      "name": "row_header",
      "type": "group",
      "role": "row-header",
      "from": {"data": "facet_domain_row"},
      "encode": {"update": {"height": {"signal": "child_height"}}},
      "axes": [
        {
          "scale": "y",
          "orient": "left",
          "grid": false,
          "title": "Female_Percentage",
          "labelOverlap": true,
          "tickCount": {"signal": "ceil(child_height/40)"},
          "zindex": 0
        }
      ]
    },
    {
      "name": "column_footer",
      "type": "group",
      "role": "column-footer",
      "from": {"data": "facet_domain_column"},
      "encode": {"update": {"width": {"signal": "child_width"}}},
      "axes": [
        {
          "scale": "x",
          "orient": "bottom",
          "grid": false,
          "title": "Year",
          "labelFlush": true,
          "labelOverlap": true,
          "tickCount": {"signal": "ceil(child_width/40)"},
          "zindex": 0
        }
      ]
    },
    {
      "name": "cell",
      "type": "group",
      "title": {
        "text": {
          "signal": "isValid(parent[\"Continent\"]) ? parent[\"Continent\"] : \"\"+parent[\"Continent\"]"
        },
        "style": "guide-label",
        "frame": "group",
        "offset": 10
      },
      "style": "cell",
      "from": {
        "facet": {"name": "facet", "data": "data_0", "groupby": ["Continent"]}
      },
      "sort": {"field": ["datum[\"Continent\"]"], "order": ["ascending"]},
      "encode": {
        "update": {
          "width": {"signal": "child_width"},
          "height": {"signal": "child_height"}
        }
      },
      "signals": [
        {
          "name": "facet",
          "value": {},
          "on": [
            {
              "events": [{"source": "scope", "type": "mousemove"}],
              "update": "isTuple(facet) ? facet : group(\"cell\").datum"
            }
          ]
        },
        {
          "name": "selector069_Year",
          "on": [
            {
              "events": {"signal": "selector069_translate_delta"},
              "update": "panLinear(selector069_translate_anchor.extent_x, -selector069_translate_delta.x / child_width)"
            },
            {
              "events": {"signal": "selector069_zoom_delta"},
              "update": "zoomLinear(domain(\"x\"), selector069_zoom_anchor.x, selector069_zoom_delta)"
            },
            {
              "events": [{"source": "scope", "type": "dblclick"}],
              "update": "null"
            }
          ],
          "push": "outer"
        },
        {
          "name": "selector069_Female_Percentage",
          "on": [
            {
              "events": {"signal": "selector069_translate_delta"},
              "update": "panLinear(selector069_translate_anchor.extent_y, selector069_translate_delta.y / child_height)"
            },
            {
              "events": {"signal": "selector069_zoom_delta"},
              "update": "zoomLinear(domain(\"y\"), selector069_zoom_anchor.y, selector069_zoom_delta)"
            },
            {
              "events": [{"source": "scope", "type": "dblclick"}],
              "update": "null"
            }
          ],
          "push": "outer"
        },
        {
          "name": "selector069_tuple",
          "on": [
            {
              "events": [
                {"signal": "selector069_Year || selector069_Female_Percentage"}
              ],
              "update": "selector069_Year && selector069_Female_Percentage ? {unit: \"child\" + '__facet_facet_' + (facet[\"Continent\"]), fields: selector069_tuple_fields, values: [selector069_Year,selector069_Female_Percentage]} : null"
            }
          ]
        },
        {
          "name": "selector069_tuple_fields",
          "value": [
            {"field": "Year", "channel": "x", "type": "R"},
            {"field": "Female_Percentage", "channel": "y", "type": "R"}
          ]
        },
        {
          "name": "selector069_translate_anchor",
          "value": {},
          "on": [
            {
              "events": [{"source": "scope", "type": "mousedown"}],
              "update": "{x: x(unit), y: y(unit), extent_x: domain(\"x\"), extent_y: domain(\"y\")}"
            }
          ]
        },
        {
          "name": "selector069_translate_delta",
          "value": {},
          "on": [
            {
              "events": [
                {
                  "source": "window",
                  "type": "mousemove",
                  "consume": true,
                  "between": [
                    {"source": "scope", "type": "mousedown"},
                    {"source": "window", "type": "mouseup"}
                  ]
                }
              ],
              "update": "{x: selector069_translate_anchor.x - x(unit), y: selector069_translate_anchor.y - y(unit)}"
            }
          ]
        },
        {
          "name": "selector069_zoom_anchor",
          "on": [
            {
              "events": [{"source": "scope", "type": "wheel", "consume": true}],
              "update": "{x: invert(\"x\", x(unit)), y: invert(\"y\", y(unit))}"
            }
          ]
        },
        {
          "name": "selector069_zoom_delta",
          "on": [
            {
              "events": [{"source": "scope", "type": "wheel", "consume": true}],
              "force": true,
              "update": "pow(1.001, event.deltaY * pow(16, event.deltaMode))"
            }
          ]
        },
        {
          "name": "selector069_modify",
          "on": [
            {
              "events": {"signal": "selector069_tuple"},
              "update": "modify(\"selector069_store\", selector069_tuple, true)"
            }
          ]
        }
      ],
      "marks": [
        {
          "name": "child_pathgroup",
          "type": "group",
          "from": {
            "facet": {
              "name": "faceted_path_child_main",
              "data": "facet",
              "groupby": ["Continent"]
            }
          },
          "encode": {
            "update": {
              "width": {"field": {"group": "width"}},
              "height": {"field": {"group": "height"}}
            }
          },
          "marks": [
            {
              "name": "child_marks",
              "type": "line",
              "clip": true,
              "style": ["line"],
              "sort": {"field": "datum[\"Year\"]"},
              "interactive": true,
              "from": {"data": "faceted_path_child_main"},
              "encode": {
                "update": {
                  "stroke": {"scale": "color", "field": "Continent"},
                  "tooltip": {
                    "signal": "{\"Year\": format(datum[\"Year\"], \"\"), \"Continent\": isValid(datum[\"Continent\"]) ? datum[\"Continent\"] : \"\"+datum[\"Continent\"], \"Female Percentage\": isValid(datum[\"Female Percentage\"]) ? datum[\"Female Percentage\"] : \"\"+datum[\"Female Percentage\"]}"
                  },
                  "description": {
                    "signal": "\"Continent\" + \": \" + (isValid(datum[\"Continent\"]) ? datum[\"Continent\"] : \"\"+datum[\"Continent\"]) + \"; \" + \"Year\" + \": \" + (format(datum[\"Year\"], \"\")) + \"; \" + \"Female Percentage\" + \": \" + (isValid(datum[\"Female Percentage\"]) ? datum[\"Female Percentage\"] : \"\"+datum[\"Female Percentage\"]) + \"; \" + \"Female_Percentage\" + \": \" + (format(datum[\"Female_Percentage\"], \"\"))"
                  },
                  "x": {"scale": "x", "field": "Year"},
                  "y": {"scale": "y", "field": "Female_Percentage"},
                  "strokeWidth": {"value": 5},
                  "defined": {
                    "signal": "isValid(datum[\"Year\"]) && isFinite(+datum[\"Year\"]) && isValid(datum[\"Female_Percentage\"]) && isFinite(+datum[\"Female_Percentage\"])"
                  }
                }
              }
            }
          ]
        }
      ],
      "axes": [
        {
          "scale": "x",
          "orient": "bottom",
          "gridScale": "y",
          "grid": true,
          "tickCount": {"signal": "ceil(child_width/40)"},
          "domain": false,
          "labels": false,
          "aria": false,
          "maxExtent": 0,
          "minExtent": 0,
          "ticks": false,
          "zindex": 0
        },
        {
          "scale": "y",
          "orient": "left",
          "gridScale": "x",
          "grid": true,
          "tickCount": {"signal": "ceil(child_height/40)"},
          "domain": false,
          "labels": false,
          "aria": false,
          "maxExtent": 0,
          "minExtent": 0,
          "ticks": false,
          "zindex": 0
        }
      ]
    }
  ],
  "scales": [
    {
      "name": "x",
      "type": "linear",
      "domain": {"data": "data_0", "field": "Year"},
      "domainRaw": {"signal": "selector069[\"Year\"]"},
      "range": [0, {"signal": "child_width"}],
      "nice": true,
      "zero": false
    },
    {
      "name": "y",
      "type": "linear",
      "domain": {"data": "data_0", "field": "Female_Percentage"},
      "domainRaw": {"signal": "selector069[\"Female_Percentage\"]"},
      "range": [{"signal": "child_height"}, 0],
      "nice": true,
      "zero": true
    },
    {
      "name": "color",
      "type": "ordinal",
      "domain": {"data": "data_0", "field": "Continent", "sort": true},
      "range": "category"
    }
  ],
  "legends": [
    {"stroke": "color", "symbolType": "stroke", "title": "Continent"}
  ],
  "config": {"style": {"group-title": {"fontSize": 18, "fill": "black"}}}
}

vegaEmbed('#figure28_2', figure28_2);
</script>

<script type="text/javascript">
var figure29 = {
  "$schema": "https://vega.github.io/schema/vega/v5.json",
  "background": "white",
  "padding": 5,
  "title": {
    "text": "Changes in female athletes participation in Summer Olympics",
    "anchor": "middle"
  },
  "data": [
    {"name": "selector072_store"},
    {
      "name": "data-c9cd4958aa454941ccfb344427499b56",
      "values": [
        {
          "Year": 1896,
          "Continent": "Global",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1900,
          "Continent": "Global",
          "Female_Percentage": 0.016045548654244308,
          "Female Percentage": "1.6%"
        },
        {
          "Year": 1904,
          "Continent": "Global",
          "Female_Percentage": 0.012307692307692308,
          "Female Percentage": "1.2%"
        },
        {
          "Year": 1906,
          "Continent": "Global",
          "Female_Percentage": 0.006489675516224189,
          "Female Percentage": "0.6%"
        },
        {
          "Year": 1908,
          "Continent": "Global",
          "Female_Percentage": 0.015568068896985756,
          "Female Percentage": "1.6%"
        },
        {
          "Year": 1912,
          "Continent": "Global",
          "Female_Percentage": 0.020242914979757085,
          "Female Percentage": "2.0%"
        },
        {
          "Year": 1920,
          "Continent": "Global",
          "Female_Percentage": 0.03247863247863248,
          "Female Percentage": "3.2%"
        },
        {
          "Year": 1924,
          "Continent": "Global",
          "Female_Percentage": 0.04917363803305448,
          "Female Percentage": "4.9%"
        },
        {
          "Year": 1928,
          "Continent": "Global",
          "Female_Percentage": 0.08397582829756199,
          "Female Percentage": "8.4%"
        },
        {
          "Year": 1932,
          "Continent": "Global",
          "Female_Percentage": 0.11859193438140808,
          "Female Percentage": "11.9%"
        },
        {
          "Year": 1936,
          "Continent": "Global",
          "Female_Percentage": 0.07177974434611603,
          "Female Percentage": "7.2%"
        },
        {
          "Year": 1948,
          "Continent": "Global",
          "Female_Percentage": 0.0974740932642487,
          "Female Percentage": "9.7%"
        },
        {
          "Year": 1952,
          "Continent": "Global",
          "Female_Percentage": 0.17301414581066374,
          "Female Percentage": "17.3%"
        },
        {
          "Year": 1956,
          "Continent": "Global",
          "Female_Percentage": 0.1704136690647482,
          "Female Percentage": "17.0%"
        },
        {
          "Year": 1960,
          "Continent": "Global",
          "Female_Percentage": 0.1761111111111111,
          "Female Percentage": "17.6%"
        },
        {
          "Year": 1964,
          "Continent": "Global",
          "Female_Percentage": 0.17183667580435724,
          "Female Percentage": "17.2%"
        },
        {
          "Year": 1968,
          "Continent": "Global",
          "Female_Percentage": 0.19755020652328728,
          "Female Percentage": "19.8%"
        },
        {
          "Year": 1972,
          "Continent": "Global",
          "Female_Percentage": 0.2010383965225791,
          "Female Percentage": "20.1%"
        },
        {
          "Year": 1976,
          "Continent": "Global",
          "Female_Percentage": 0.2333720592506535,
          "Female Percentage": "23.3%"
        },
        {
          "Year": 1980,
          "Continent": "Global",
          "Female_Percentage": 0.22398271516024487,
          "Female Percentage": "22.4%"
        },
        {
          "Year": 1984,
          "Continent": "Global",
          "Female_Percentage": 0.25244707489187346,
          "Female Percentage": "25.2%"
        },
        {
          "Year": 1988,
          "Continent": "Global",
          "Female_Percentage": 0.2830937035200793,
          "Female Percentage": "28.3%"
        },
        {
          "Year": 1992,
          "Continent": "Global",
          "Female_Percentage": 0.3129472457979697,
          "Female Percentage": "31.3%"
        },
        {
          "Year": 1996,
          "Continent": "Global",
          "Female_Percentage": 0.36325520654340493,
          "Female Percentage": "36.3%"
        },
        {
          "Year": 2000,
          "Continent": "Global",
          "Female_Percentage": 0.3939145299145299,
          "Female Percentage": "39.4%"
        },
        {
          "Year": 2004,
          "Continent": "Global",
          "Female_Percentage": 0.4132602893664841,
          "Female Percentage": "41.3%"
        },
        {
          "Year": 2008,
          "Continent": "Global",
          "Female_Percentage": 0.4284037558685446,
          "Female Percentage": "42.8%"
        },
        {
          "Year": 2012,
          "Continent": "Global",
          "Female_Percentage": 0.4500399100210435,
          "Female Percentage": "45.0%"
        },
        {
          "Year": 2016,
          "Continent": "Global",
          "Female_Percentage": 0.4535101729046594,
          "Female Percentage": "45.4%"
        },
        {
          "Year": 1896,
          "Continent": "Africa",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1900,
          "Continent": "Africa",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1904,
          "Continent": "Africa",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1906,
          "Continent": "Africa",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1908,
          "Continent": "Africa",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1912,
          "Continent": "Africa",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1920,
          "Continent": "Africa",
          "Female_Percentage": 0.01680672268907563,
          "Female Percentage": "1.7%"
        },
        {
          "Year": 1924,
          "Continent": "Africa",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1928,
          "Continent": "Africa",
          "Female_Percentage": 0.1411764705882353,
          "Female Percentage": "14.1%"
        },
        {
          "Year": 1932,
          "Continent": "Africa",
          "Female_Percentage": 0.25,
          "Female Percentage": "25.0%"
        },
        {
          "Year": 1936,
          "Continent": "Africa",
          "Female_Percentage": 0.1,
          "Female Percentage": "10.0%"
        },
        {
          "Year": 1948,
          "Continent": "Africa",
          "Female_Percentage": 0.009569377990430622,
          "Female Percentage": "1.0%"
        },
        {
          "Year": 1952,
          "Continent": "Africa",
          "Female_Percentage": 0.02735562310030395,
          "Female Percentage": "2.7%"
        },
        {
          "Year": 1956,
          "Continent": "Africa",
          "Female_Percentage": 0.0748663101604278,
          "Female Percentage": "7.5%"
        },
        {
          "Year": 1960,
          "Continent": "Africa",
          "Female_Percentage": 0.04456824512534819,
          "Female Percentage": "4.5%"
        },
        {
          "Year": 1964,
          "Continent": "Africa",
          "Female_Percentage": 0.045454545454545456,
          "Female Percentage": "4.5%"
        },
        {
          "Year": 1968,
          "Continent": "Africa",
          "Female_Percentage": 0.039886039886039885,
          "Female Percentage": "4.0%"
        },
        {
          "Year": 1972,
          "Continent": "Africa",
          "Female_Percentage": 0.056985294117647065,
          "Female Percentage": "5.7%"
        },
        {
          "Year": 1976,
          "Continent": "Africa",
          "Female_Percentage": 0.0707070707070707,
          "Female Percentage": "7.1%"
        },
        {
          "Year": 1980,
          "Continent": "Africa",
          "Female_Percentage": 0.1524590163934426,
          "Female Percentage": "15.2%"
        },
        {
          "Year": 1984,
          "Continent": "Africa",
          "Female_Percentage": 0.09419354838709676,
          "Female Percentage": "9.4%"
        },
        {
          "Year": 1988,
          "Continent": "Africa",
          "Female_Percentage": 0.13974799541809851,
          "Female Percentage": "14.0%"
        },
        {
          "Year": 1992,
          "Continent": "Africa",
          "Female_Percentage": 0.22341568206229864,
          "Female Percentage": "22.3%"
        },
        {
          "Year": 1996,
          "Continent": "Africa",
          "Female_Percentage": 0.2462077012835473,
          "Female Percentage": "24.6%"
        },
        {
          "Year": 2000,
          "Continent": "Africa",
          "Female_Percentage": 0.3296370967741936,
          "Female Percentage": "33.0%"
        },
        {
          "Year": 2004,
          "Continent": "Africa",
          "Female_Percentage": 0.33407572383073497,
          "Female Percentage": "33.4%"
        },
        {
          "Year": 2008,
          "Continent": "Africa",
          "Female_Percentage": 0.3874734607218684,
          "Female Percentage": "38.7%"
        },
        {
          "Year": 2012,
          "Continent": "Africa",
          "Female_Percentage": 0.399581589958159,
          "Female Percentage": "40.0%"
        },
        {
          "Year": 2016,
          "Continent": "Africa",
          "Female_Percentage": 0.3836772983114447,
          "Female Percentage": "38.4%"
        },
        {
          "Year": 1896,
          "Continent": "Asia",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1900,
          "Continent": "Asia",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1904,
          "Continent": "Asia",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1906,
          "Continent": "Asia",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1908,
          "Continent": "Asia",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1912,
          "Continent": "Asia",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1920,
          "Continent": "Asia",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1924,
          "Continent": "Asia",
          "Female_Percentage": 0.033707865168539325,
          "Female Percentage": "3.4%"
        },
        {
          "Year": 1928,
          "Continent": "Asia",
          "Female_Percentage": 0.015873015873015872,
          "Female Percentage": "1.6%"
        },
        {
          "Year": 1932,
          "Continent": "Asia",
          "Female_Percentage": 0.11203319502074688,
          "Female Percentage": "11.2%"
        },
        {
          "Year": 1936,
          "Continent": "Asia",
          "Female_Percentage": 0.057620817843866176,
          "Female Percentage": "5.8%"
        },
        {
          "Year": 1948,
          "Continent": "Asia",
          "Female_Percentage": 0.0069124423963133645,
          "Female Percentage": "0.7%"
        },
        {
          "Year": 1952,
          "Continent": "Asia",
          "Female_Percentage": 0.065439672801636,
          "Female Percentage": "6.5%"
        },
        {
          "Year": 1956,
          "Continent": "Asia",
          "Female_Percentage": 0.1060126582278481,
          "Female Percentage": "10.6%"
        },
        {
          "Year": 1960,
          "Continent": "Asia",
          "Female_Percentage": 0.129366106080207,
          "Female Percentage": "12.9%"
        },
        {
          "Year": 1964,
          "Continent": "Asia",
          "Female_Percentage": 0.14587593728698026,
          "Female Percentage": "14.6%"
        },
        {
          "Year": 1968,
          "Continent": "Asia",
          "Female_Percentage": 0.17119244391971666,
          "Female Percentage": "17.1%"
        },
        {
          "Year": 1972,
          "Continent": "Asia",
          "Female_Percentage": 0.14781746031746032,
          "Female Percentage": "14.8%"
        },
        {
          "Year": 1976,
          "Continent": "Asia",
          "Female_Percentage": 0.16761041902604756,
          "Female Percentage": "16.8%"
        },
        {
          "Year": 1980,
          "Continent": "Asia",
          "Female_Percentage": 0.1494661921708185,
          "Female Percentage": "14.9%"
        },
        {
          "Year": 1984,
          "Continent": "Asia",
          "Female_Percentage": 0.2409855769230769,
          "Female Percentage": "24.1%"
        },
        {
          "Year": 1988,
          "Continent": "Asia",
          "Female_Percentage": 0.3037466547725245,
          "Female Percentage": "30.4%"
        },
        {
          "Year": 1992,
          "Continent": "Asia",
          "Female_Percentage": 0.31186440677966104,
          "Female Percentage": "31.2%"
        },
        {
          "Year": 1996,
          "Continent": "Asia",
          "Female_Percentage": 0.3821571238348868,
          "Female Percentage": "38.2%"
        },
        {
          "Year": 2000,
          "Continent": "Asia",
          "Female_Percentage": 0.39642620780939775,
          "Female Percentage": "39.6%"
        },
        {
          "Year": 2004,
          "Continent": "Asia",
          "Female_Percentage": 0.4359058207979071,
          "Female Percentage": "43.6%"
        },
        {
          "Year": 2008,
          "Continent": "Asia",
          "Female_Percentage": 0.43423423423423424,
          "Female Percentage": "43.4%"
        },
        {
          "Year": 2012,
          "Continent": "Asia",
          "Female_Percentage": 0.4599396580623533,
          "Female Percentage": "46.0%"
        },
        {
          "Year": 2016,
          "Continent": "Asia",
          "Female_Percentage": 0.4653897849462366,
          "Female Percentage": "46.5%"
        },
        {
          "Year": 1896,
          "Continent": "Europe",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1900,
          "Continent": "Europe",
          "Female_Percentage": 0.012528473804100227,
          "Female Percentage": "1.3%"
        },
        {
          "Year": 1904,
          "Continent": "Europe",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1906,
          "Continent": "Europe",
          "Female_Percentage": 0.006905210295040804,
          "Female Percentage": "0.7%"
        },
        {
          "Year": 1908,
          "Continent": "Europe",
          "Female_Percentage": 0.01800076599004213,
          "Female Percentage": "1.8%"
        },
        {
          "Year": 1912,
          "Continent": "Europe",
          "Female_Percentage": 0.024897480960749854,
          "Female Percentage": "2.5%"
        },
        {
          "Year": 1920,
          "Continent": "Europe",
          "Female_Percentage": 0.03142943487458446,
          "Female Percentage": "3.1%"
        },
        {
          "Year": 1924,
          "Continent": "Europe",
          "Female_Percentage": 0.05149330587023687,
          "Female Percentage": "5.1%"
        },
        {
          "Year": 1928,
          "Continent": "Europe",
          "Female_Percentage": 0.0821664464993395,
          "Female Percentage": "8.2%"
        },
        {
          "Year": 1932,
          "Continent": "Europe",
          "Female_Percentage": 0.10588235294117647,
          "Female Percentage": "10.6%"
        },
        {
          "Year": 1936,
          "Continent": "Europe",
          "Female_Percentage": 0.06700091157702825,
          "Female Percentage": "6.7%"
        },
        {
          "Year": 1948,
          "Continent": "Europe",
          "Female_Percentage": 0.1073929961089494,
          "Female Percentage": "10.7%"
        },
        {
          "Year": 1952,
          "Continent": "Europe",
          "Female_Percentage": 0.20599325262949,
          "Female Percentage": "20.6%"
        },
        {
          "Year": 1956,
          "Continent": "Europe",
          "Female_Percentage": 0.20808451998162608,
          "Female Percentage": "20.8%"
        },
        {
          "Year": 1960,
          "Continent": "Europe",
          "Female_Percentage": 0.19808861859252824,
          "Female Percentage": "19.8%"
        },
        {
          "Year": 1964,
          "Continent": "Europe",
          "Female_Percentage": 0.19008009858287125,
          "Female Percentage": "19.0%"
        },
        {
          "Year": 1968,
          "Continent": "Europe",
          "Female_Percentage": 0.20454545454545456,
          "Female Percentage": "20.5%"
        },
        {
          "Year": 1972,
          "Continent": "Europe",
          "Female_Percentage": 0.22300968580203165,
          "Female Percentage": "22.3%"
        },
        {
          "Year": 1976,
          "Continent": "Europe",
          "Female_Percentage": 0.2362555720653789,
          "Female Percentage": "23.6%"
        },
        {
          "Year": 1980,
          "Continent": "Europe",
          "Female_Percentage": 0.257801108194809,
          "Female Percentage": "25.8%"
        },
        {
          "Year": 1984,
          "Continent": "Europe",
          "Female_Percentage": 0.2688271604938272,
          "Female Percentage": "26.9%"
        },
        {
          "Year": 1988,
          "Continent": "Europe",
          "Female_Percentage": 0.29081000743126084,
          "Female Percentage": "29.1%"
        },
        {
          "Year": 1992,
          "Continent": "Europe",
          "Female_Percentage": 0.3262682418346073,
          "Female Percentage": "32.6%"
        },
        {
          "Year": 1996,
          "Continent": "Europe",
          "Female_Percentage": 0.3664026677782409,
          "Female Percentage": "36.6%"
        },
        {
          "Year": 2000,
          "Continent": "Europe",
          "Female_Percentage": 0.38596989491621697,
          "Female Percentage": "38.6%"
        },
        {
          "Year": 2004,
          "Continent": "Europe",
          "Female_Percentage": 0.4022806004618938,
          "Female Percentage": "40.2%"
        },
        {
          "Year": 2008,
          "Continent": "Europe",
          "Female_Percentage": 0.4252481849162839,
          "Female Percentage": "42.5%"
        },
        {
          "Year": 2012,
          "Continent": "Europe",
          "Female_Percentage": 0.4477747502270663,
          "Female Percentage": "44.8%"
        },
        {
          "Year": 2016,
          "Continent": "Europe",
          "Female_Percentage": 0.4510353417406197,
          "Female Percentage": "45.1%"
        },
        {
          "Year": 1896,
          "Continent": "North America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1900,
          "Continent": "North America",
          "Female_Percentage": 0.05960264900662252,
          "Female Percentage": "6.0%"
        },
        {
          "Year": 1904,
          "Continent": "North America",
          "Female_Percentage": 0.013605442176870748,
          "Female Percentage": "1.4%"
        },
        {
          "Year": 1906,
          "Continent": "North America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1908,
          "Continent": "North America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1912,
          "Continent": "North America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1920,
          "Continent": "North America",
          "Female_Percentage": 0.03942652329749104,
          "Female Percentage": "3.9%"
        },
        {
          "Year": 1924,
          "Continent": "North America",
          "Female_Percentage": 0.05843071786310518,
          "Female Percentage": "5.8%"
        },
        {
          "Year": 1928,
          "Continent": "North America",
          "Female_Percentage": 0.11,
          "Female Percentage": "11.0%"
        },
        {
          "Year": 1932,
          "Continent": "North America",
          "Female_Percentage": 0.14641148325358852,
          "Female Percentage": "14.6%"
        },
        {
          "Year": 1936,
          "Continent": "North America",
          "Female_Percentage": 0.1221264367816092,
          "Female Percentage": "12.2%"
        },
        {
          "Year": 1948,
          "Continent": "North America",
          "Female_Percentage": 0.11932418162618795,
          "Female Percentage": "11.9%"
        },
        {
          "Year": 1952,
          "Continent": "North America",
          "Female_Percentage": 0.16042154566744732,
          "Female Percentage": "16.0%"
        },
        {
          "Year": 1956,
          "Continent": "North America",
          "Female_Percentage": 0.19484240687679086,
          "Female Percentage": "19.5%"
        },
        {
          "Year": 1960,
          "Continent": "North America",
          "Female_Percentage": 0.21568627450980396,
          "Female Percentage": "21.6%"
        },
        {
          "Year": 1964,
          "Continent": "North America",
          "Female_Percentage": 0.2101661779081134,
          "Female Percentage": "21.0%"
        },
        {
          "Year": 1968,
          "Continent": "North America",
          "Female_Percentage": 0.2272957889396245,
          "Female Percentage": "22.7%"
        },
        {
          "Year": 1972,
          "Continent": "North America",
          "Female_Percentage": 0.23755924170616116,
          "Female Percentage": "23.8%"
        },
        {
          "Year": 1976,
          "Continent": "North America",
          "Female_Percentage": 0.27378964941569284,
          "Female Percentage": "27.4%"
        },
        {
          "Year": 1980,
          "Continent": "North America",
          "Female_Percentage": 0.17372881355932204,
          "Female Percentage": "17.4%"
        },
        {
          "Year": 1984,
          "Continent": "North America",
          "Female_Percentage": 0.3223987698616094,
          "Female Percentage": "32.2%"
        },
        {
          "Year": 1988,
          "Continent": "North America",
          "Female_Percentage": 0.32998324958123953,
          "Female Percentage": "33.0%"
        },
        {
          "Year": 1992,
          "Continent": "North America",
          "Female_Percentage": 0.3336653386454183,
          "Female Percentage": "33.4%"
        },
        {
          "Year": 1996,
          "Continent": "North America",
          "Female_Percentage": 0.3953257086026852,
          "Female Percentage": "39.5%"
        },
        {
          "Year": 2000,
          "Continent": "North America",
          "Female_Percentage": 0.4241469816272966,
          "Female Percentage": "42.4%"
        },
        {
          "Year": 2004,
          "Continent": "North America",
          "Female_Percentage": 0.4470720720720721,
          "Female Percentage": "44.7%"
        },
        {
          "Year": 2008,
          "Continent": "North America",
          "Female_Percentage": 0.4338074398249453,
          "Female Percentage": "43.4%"
        },
        {
          "Year": 2012,
          "Continent": "North America",
          "Female_Percentage": 0.4791666666666667,
          "Female Percentage": "47.9%"
        },
        {
          "Year": 2016,
          "Continent": "North America",
          "Female_Percentage": 0.4955947136563877,
          "Female Percentage": "49.6%"
        },
        {
          "Year": 1896,
          "Continent": "Oceania",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1900,
          "Continent": "Oceania",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1904,
          "Continent": "Oceania",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1906,
          "Continent": "Oceania",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1908,
          "Continent": "Oceania",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1912,
          "Continent": "Oceania",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1920,
          "Continent": "Oceania",
          "Female_Percentage": 0.14285714285714285,
          "Female Percentage": "14.3%"
        },
        {
          "Year": 1924,
          "Continent": "Oceania",
          "Female_Percentage": 0.045454545454545456,
          "Female Percentage": "4.5%"
        },
        {
          "Year": 1928,
          "Continent": "Oceania",
          "Female_Percentage": 0.2857142857142857,
          "Female Percentage": "28.6%"
        },
        {
          "Year": 1932,
          "Continent": "Oceania",
          "Female_Percentage": 0.12244897959183673,
          "Female Percentage": "12.2%"
        },
        {
          "Year": 1936,
          "Continent": "Oceania",
          "Female_Percentage": 0.125,
          "Female Percentage": "12.5%"
        },
        {
          "Year": 1948,
          "Continent": "Oceania",
          "Female_Percentage": 0.17117117117117114,
          "Female Percentage": "17.1%"
        },
        {
          "Year": 1952,
          "Continent": "Oceania",
          "Female_Percentage": 0.1375,
          "Female Percentage": "13.8%"
        },
        {
          "Year": 1956,
          "Continent": "Oceania",
          "Female_Percentage": 0.1729957805907173,
          "Female Percentage": "17.3%"
        },
        {
          "Year": 1960,
          "Continent": "Oceania",
          "Female_Percentage": 0.18787878787878787,
          "Female Percentage": "18.8%"
        },
        {
          "Year": 1964,
          "Continent": "Oceania",
          "Female_Percentage": 0.2375,
          "Female Percentage": "23.8%"
        },
        {
          "Year": 1968,
          "Continent": "Oceania",
          "Female_Percentage": 0.25862068965517243,
          "Female Percentage": "25.9%"
        },
        {
          "Year": 1972,
          "Continent": "Oceania",
          "Female_Percentage": 0.2356020942408377,
          "Female Percentage": "23.6%"
        },
        {
          "Year": 1976,
          "Continent": "Oceania",
          "Female_Percentage": 0.2383419689119171,
          "Female Percentage": "23.8%"
        },
        {
          "Year": 1980,
          "Continent": "Oceania",
          "Female_Percentage": 0.29949238578680204,
          "Female Percentage": "29.9%"
        },
        {
          "Year": 1984,
          "Continent": "Oceania",
          "Female_Percentage": 0.2949640287769784,
          "Female Percentage": "29.5%"
        },
        {
          "Year": 1988,
          "Continent": "Oceania",
          "Female_Percentage": 0.2690972222222222,
          "Female Percentage": "26.9%"
        },
        {
          "Year": 1992,
          "Continent": "Oceania",
          "Female_Percentage": 0.3381712626995646,
          "Female Percentage": "33.8%"
        },
        {
          "Year": 1996,
          "Continent": "Oceania",
          "Female_Percentage": 0.3949801849405548,
          "Female Percentage": "39.5%"
        },
        {
          "Year": 2000,
          "Continent": "Oceania",
          "Female_Percentage": 0.4650934119960669,
          "Female Percentage": "46.5%"
        },
        {
          "Year": 2004,
          "Continent": "Oceania",
          "Female_Percentage": 0.4480286738351255,
          "Female Percentage": "44.8%"
        },
        {
          "Year": 2008,
          "Continent": "Oceania",
          "Female_Percentage": 0.4597839135654262,
          "Female Percentage": "46.0%"
        },
        {
          "Year": 2012,
          "Continent": "Oceania",
          "Female_Percentage": 0.4623115577889447,
          "Female Percentage": "46.2%"
        },
        {
          "Year": 2016,
          "Continent": "Oceania",
          "Female_Percentage": 0.4833141542002302,
          "Female Percentage": "48.3%"
        },
        {
          "Year": 1896,
          "Continent": "South America",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1900,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1904,
          "Continent": "South America",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1906,
          "Continent": "South America",
          "Female_Percentage": null,
          "Female Percentage": "nan%"
        },
        {
          "Year": 1908,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1912,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1920,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1924,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1928,
          "Continent": "South America",
          "Female_Percentage": 0,
          "Female Percentage": "0.0%"
        },
        {
          "Year": 1932,
          "Continent": "South America",
          "Female_Percentage": 0.023809523809523808,
          "Female Percentage": "2.4%"
        },
        {
          "Year": 1936,
          "Continent": "South America",
          "Female_Percentage": 0.03205128205128205,
          "Female Percentage": "3.2%"
        },
        {
          "Year": 1948,
          "Continent": "South America",
          "Female_Percentage": 0.08225806451612902,
          "Female Percentage": "8.2%"
        },
        {
          "Year": 1952,
          "Continent": "South America",
          "Female_Percentage": 0.07068607068607069,
          "Female Percentage": "7.1%"
        },
        {
          "Year": 1956,
          "Continent": "South America",
          "Female_Percentage": 0.021428571428571432,
          "Female Percentage": "2.1%"
        },
        {
          "Year": 1960,
          "Continent": "South America",
          "Female_Percentage": 0.03523035230352303,
          "Female Percentage": "3.5%"
        },
        {
          "Year": 1964,
          "Continent": "South America",
          "Female_Percentage": 0.04132231404958678,
          "Female Percentage": "4.1%"
        },
        {
          "Year": 1968,
          "Continent": "South America",
          "Female_Percentage": 0.15560165975103735,
          "Female Percentage": "15.6%"
        },
        {
          "Year": 1972,
          "Continent": "South America",
          "Female_Percentage": 0.117096018735363,
          "Female Percentage": "11.7%"
        },
        {
          "Year": 1976,
          "Continent": "South America",
          "Female_Percentage": 0.2050561797752809,
          "Female Percentage": "20.5%"
        },
        {
          "Year": 1980,
          "Continent": "South America",
          "Female_Percentage": 0.14788732394366194,
          "Female Percentage": "14.8%"
        },
        {
          "Year": 1984,
          "Continent": "South America",
          "Female_Percentage": 0.13333333333333333,
          "Female Percentage": "13.3%"
        },
        {
          "Year": 1988,
          "Continent": "South America",
          "Female_Percentage": 0.2332155477031802,
          "Female Percentage": "23.3%"
        },
        {
          "Year": 1992,
          "Continent": "South America",
          "Female_Percentage": 0.2249560632688928,
          "Female Percentage": "22.5%"
        },
        {
          "Year": 1996,
          "Continent": "South America",
          "Female_Percentage": 0.2697095435684647,
          "Female Percentage": "27.0%"
        },
        {
          "Year": 2000,
          "Continent": "South America",
          "Female_Percentage": 0.366306027820711,
          "Female Percentage": "36.6%"
        },
        {
          "Year": 2004,
          "Continent": "South America",
          "Female_Percentage": 0.39811066126855604,
          "Female Percentage": "39.8%"
        },
        {
          "Year": 2008,
          "Continent": "South America",
          "Female_Percentage": 0.4339152119700748,
          "Female Percentage": "43.4%"
        },
        {
          "Year": 2012,
          "Continent": "South America",
          "Female_Percentage": 0.4207920792079208,
          "Female Percentage": "42.1%"
        },
        {
          "Year": 2016,
          "Continent": "South America",
          "Female_Percentage": 0.4156674660271783,
          "Female Percentage": "41.6%"
        }
      ]
    },
    {
      "name": "data_0",
      "source": "data-c9cd4958aa454941ccfb344427499b56",
      "transform": [
        {"type": "formula", "expr": "toNumber(datum[\"Year\"])", "as": "Year"},
        {"type": "filter", "expr": "(datum.symbol !== 'GOOG')"}
      ]
    },
    {
      "name": "row_domain",
      "source": "data_0",
      "transform": [{"type": "aggregate", "groupby": ["Continent"]}]
    }
  ],
  "signals": [
    {"name": "child_width", "value": 550},
    {"name": "child_height", "value": 80},
    {
      "name": "unit",
      "value": {},
      "on": [
        {"events": "mousemove", "update": "isTuple(group()) ? group() : unit"}
      ]
    },
    {
      "name": "selector072",
      "update": "{\"Year\": selector072_Year, \"Female_Percentage\": selector072_Female_Percentage}"
    },
    {"name": "selector072_Year"},
    {"name": "selector072_Female_Percentage"}
  ],
  "layout": {
    "padding": 20,
    "offset": {"rowTitle": 10},
    "columns": 1,
    "bounds": "full",
    "align": "all"
  },
  "marks": [
    {
      "name": "row-title",
      "type": "group",
      "role": "row-title",
      "title": {
        "text": "Continent",
        "orient": "left",
        "style": "guide-title",
        "offset": 10
      }
    },
    {
      "name": "row_header",
      "type": "group",
      "role": "row-header",
      "from": {"data": "row_domain"},
      "sort": {"field": "datum[\"Continent\"]", "order": "ascending"},
      "title": {
        "text": {
          "signal": "isValid(parent[\"Continent\"]) ? parent[\"Continent\"] : \"\"+parent[\"Continent\"]"
        },
        "orient": "left",
        "style": "guide-label",
        "frame": "group",
        "offset": 10
      },
      "encode": {"update": {"height": {"signal": "child_height"}}},
      "axes": [
        {
          "scale": "y",
          "orient": "left",
          "grid": false,
          "title": "Percentage",
          "labelOverlap": true,
          "tickCount": {"signal": "ceil(child_height/40)"},
          "zindex": 0
        }
      ]
    },
    {
      "name": "column_footer",
      "type": "group",
      "role": "column-footer",
      "encode": {"update": {"width": {"signal": "child_width"}}},
      "axes": [
        {
          "scale": "x",
          "orient": "bottom",
          "grid": false,
          "title": "Year",
          "labelFlush": true,
          "labelOverlap": true,
          "tickCount": {"signal": "ceil(child_width/40)"},
          "zindex": 0
        }
      ]
    },
    {
      "name": "cell",
      "type": "group",
      "style": "cell",
      "from": {
        "facet": {"name": "facet", "data": "data_0", "groupby": ["Continent"]}
      },
      "sort": {"field": ["datum[\"Continent\"]"], "order": ["ascending"]},
      "encode": {
        "update": {
          "width": {"signal": "child_width"},
          "height": {"signal": "child_height"}
        }
      },
      "signals": [
        {
          "name": "facet",
          "value": {},
          "on": [
            {
              "events": [{"source": "scope", "type": "mousemove"}],
              "update": "isTuple(facet) ? facet : group(\"cell\").datum"
            }
          ]
        },
        {
          "name": "selector072_Year",
          "on": [
            {
              "events": {"signal": "selector072_translate_delta"},
              "update": "panLinear(selector072_translate_anchor.extent_x, -selector072_translate_delta.x / child_width)"
            },
            {
              "events": {"signal": "selector072_zoom_delta"},
              "update": "zoomLinear(domain(\"x\"), selector072_zoom_anchor.x, selector072_zoom_delta)"
            },
            {
              "events": [{"source": "scope", "type": "dblclick"}],
              "update": "null"
            }
          ],
          "push": "outer"
        },
        {
          "name": "selector072_Female_Percentage",
          "on": [
            {
              "events": {"signal": "selector072_translate_delta"},
              "update": "panLinear(selector072_translate_anchor.extent_y, selector072_translate_delta.y / child_height)"
            },
            {
              "events": {"signal": "selector072_zoom_delta"},
              "update": "zoomLinear(domain(\"y\"), selector072_zoom_anchor.y, selector072_zoom_delta)"
            },
            {
              "events": [{"source": "scope", "type": "dblclick"}],
              "update": "null"
            }
          ],
          "push": "outer"
        },
        {
          "name": "selector072_tuple",
          "on": [
            {
              "events": [
                {"signal": "selector072_Year || selector072_Female_Percentage"}
              ],
              "update": "selector072_Year && selector072_Female_Percentage ? {unit: \"child\" + '__facet_row_' + (facet[\"Continent\"]), fields: selector072_tuple_fields, values: [selector072_Year,selector072_Female_Percentage]} : null"
            }
          ]
        },
        {
          "name": "selector072_tuple_fields",
          "value": [
            {"field": "Year", "channel": "x", "type": "R"},
            {"field": "Female_Percentage", "channel": "y", "type": "R"}
          ]
        },
        {
          "name": "selector072_translate_anchor",
          "value": {},
          "on": [
            {
              "events": [{"source": "scope", "type": "mousedown"}],
              "update": "{x: x(unit), y: y(unit), extent_x: domain(\"x\"), extent_y: domain(\"y\")}"
            }
          ]
        },
        {
          "name": "selector072_translate_delta",
          "value": {},
          "on": [
            {
              "events": [
                {
                  "source": "window",
                  "type": "mousemove",
                  "consume": true,
                  "between": [
                    {"source": "scope", "type": "mousedown"},
                    {"source": "window", "type": "mouseup"}
                  ]
                }
              ],
              "update": "{x: selector072_translate_anchor.x - x(unit), y: selector072_translate_anchor.y - y(unit)}"
            }
          ]
        },
        {
          "name": "selector072_zoom_anchor",
          "on": [
            {
              "events": [{"source": "scope", "type": "wheel", "consume": true}],
              "update": "{x: invert(\"x\", x(unit)), y: invert(\"y\", y(unit))}"
            }
          ]
        },
        {
          "name": "selector072_zoom_delta",
          "on": [
            {
              "events": [{"source": "scope", "type": "wheel", "consume": true}],
              "force": true,
              "update": "pow(1.001, event.deltaY * pow(16, event.deltaMode))"
            }
          ]
        },
        {
          "name": "selector072_modify",
          "on": [
            {
              "events": {"signal": "selector072_tuple"},
              "update": "modify(\"selector072_store\", selector072_tuple, true)"
            }
          ]
        }
      ],
      "marks": [
        {
          "name": "child_pathgroup",
          "type": "group",
          "from": {
            "facet": {
              "name": "faceted_path_child_main",
              "data": "facet",
              "groupby": ["Continent"]
            }
          },
          "encode": {
            "update": {
              "width": {"field": {"group": "width"}},
              "height": {"field": {"group": "height"}}
            }
          },
          "marks": [
            {
              "name": "child_marks",
              "type": "area",
              "clip": true,
              "style": ["area"],
              "sort": {"field": "datum[\"Year\"]"},
              "interactive": true,
              "from": {"data": "faceted_path_child_main"},
              "encode": {
                "update": {
                  "orient": {"value": "vertical"},
                  "fill": {"scale": "color", "field": "Continent"},
                  "tooltip": {
                    "signal": "{\"Year\": format(datum[\"Year\"], \"\"), \"Continent\": isValid(datum[\"Continent\"]) ? datum[\"Continent\"] : \"\"+datum[\"Continent\"], \"Female Percentage\": isValid(datum[\"Female Percentage\"]) ? datum[\"Female Percentage\"] : \"\"+datum[\"Female Percentage\"]}"
                  },
                  "description": {
                    "signal": "\"Continent\" + \": \" + (isValid(datum[\"Continent\"]) ? datum[\"Continent\"] : \"\"+datum[\"Continent\"]) + \"; \" + \"Year\" + \": \" + (format(datum[\"Year\"], \"\")) + \"; \" + \"Female Percentage\" + \": \" + (isValid(datum[\"Female Percentage\"]) ? datum[\"Female Percentage\"] : \"\"+datum[\"Female Percentage\"]) + \"; \" + \"Percentage\" + \": \" + (format(datum[\"Female_Percentage\"], \"\"))"
                  },
                  "x": {"scale": "x", "field": "Year"},
                  "y": {"scale": "y", "field": "Female_Percentage"},
                  "y2": {"scale": "y", "value": 0},
                  "defined": {
                    "signal": "isValid(datum[\"Year\"]) && isFinite(+datum[\"Year\"]) && isValid(datum[\"Female_Percentage\"]) && isFinite(+datum[\"Female_Percentage\"])"
                  }
                }
              }
            }
          ]
        }
      ],
      "axes": [
        {
          "scale": "x",
          "orient": "bottom",
          "gridScale": "y",
          "grid": true,
          "tickCount": {"signal": "ceil(child_width/40)"},
          "domain": false,
          "labels": false,
          "aria": false,
          "maxExtent": 0,
          "minExtent": 0,
          "ticks": false,
          "zindex": 0
        },
        {
          "scale": "y",
          "orient": "left",
          "gridScale": "x",
          "grid": true,
          "tickCount": {"signal": "ceil(child_height/40)"},
          "domain": false,
          "labels": false,
          "aria": false,
          "maxExtent": 0,
          "minExtent": 0,
          "ticks": false,
          "zindex": 0
        }
      ]
    }
  ],
  "scales": [
    {
      "name": "x",
      "type": "linear",
      "domain": {"data": "data_0", "field": "Year"},
      "domainRaw": {"signal": "selector072[\"Year\"]"},
      "range": [0, {"signal": "child_width"}],
      "nice": true,
      "zero": false
    },
    {
      "name": "y",
      "type": "linear",
      "domain": {"data": "data_0", "field": "Female_Percentage"},
      "domainRaw": {"signal": "selector072[\"Female_Percentage\"]"},
      "range": [{"signal": "child_height"}, 0],
      "nice": true,
      "zero": true
    },
    {
      "name": "color",
      "type": "ordinal",
      "domain": {"data": "data_0", "field": "Continent", "sort": true},
      "range": "category"
    }
  ],
  "legends": [{"fill": "color", "symbolType": "circle", "title": "Continent"}],
  "config": {
    "legend": {
      "cornerRadius": 10,
      "fillColor": "#EEEEEE",
      "labelFontSize": 14,
      "padding": 10,
      "strokeColor": "gray"
    },
    "style": {"group-title": {"fontSize": 18, "fill": "black"}},
    "axis": {"labelFontSize": 15, "titleFontSize": 12}
  }
}

vegaEmbed('#figure29', figure29);
</script>

