# Network Datasets for Introduction to Network Analysis

This repository contains all network datasets used in the textbook *Introduction to Network Analysis* by William Lamberti. Each network is stored as a pair of CSV files:
- `{name}_edges.csv` — edge list with columns `from`, `to` (and optionally `weight`)
- `{name}_nodes.csv` — node list with columns `id`, `name` (and optional attributes)

All datasets can be loaded in base R without any external packages:
```r
edges <- read.csv("social/karate_edges.csv")
nodes <- read.csv("social/karate_nodes.csv")
```

## Download

Clone this repository or download the ZIP:
```bash
git clone https://github.com/billyl320/network_data.git
```

## Dataset Index

| Name | Category | Nodes | Edges | Directed | Citation |
|------|----------|-------|-------|----------|----------|
| `animal/ants_1` | animal | 16 | 200 | Yes | [†] |
| `animal/ants_2` | animal | 13 | 361 | Yes | [‡] |
| `animal/dolphins_1` | animal | 13 | 45 | No | [†] |
| `animal/macaque` | animal | 62 | 1187 | Yes | [†] |
| `infrastructure/euroroad` | infrastructure | 1174 | 1417 | No | [‡] |
| `infrastructure/powergrid` | infrastructure | 4941 | 6594 | No | [‡] |
| `infrastructure/us_flights` | infrastructure | 276 | 2682 | No | [‡] |
| `moviegalaxies/american_beauty` | moviegalaxies | 22 | 46 | No | [§] |
| `moviegalaxies/american_history_x` | moviegalaxies | 39 | 114 | No | [§] |
| `moviegalaxies/apocalypse_now` | moviegalaxies | 40 | 211 | No | [§] |
| `moviegalaxies/blade_runner` | moviegalaxies | 25 | 44 | No | [§] |
| `moviegalaxies/braveheart` | moviegalaxies | 67 | 310 | No | [§] |
| `moviegalaxies/citizen_kane` | moviegalaxies | 56 | 148 | No | [§] |
| `moviegalaxies/die_hard` | moviegalaxies | 47 | 237 | No | [§] |
| `moviegalaxies/donnie_darko` | moviegalaxies | 28 | 80 | No | [§] |
| `moviegalaxies/eternal_sunshine_of_the_spotless_mind` | moviegalaxies | 32 | 69 | No | [§] |
| `moviegalaxies/fargo` | moviegalaxies | 32 | 64 | No | [§] |
| `moviegalaxies/fight_club` | moviegalaxies | 46 | 94 | No | [§] |
| `moviegalaxies/forrest_gump` | moviegalaxies | 94 | 271 | No | [§] |
| `moviegalaxies/gladiator` | moviegalaxies | 29 | 82 | No | [§] |
| `moviegalaxies/heat` | moviegalaxies | 59 | 135 | No | [§] |
| `moviegalaxies/jaws` | moviegalaxies | 36 | 85 | No | [§] |
| `moviegalaxies/jurassic_park` | moviegalaxies | 24 | 115 | No | [§] |
| `moviegalaxies/memento` | moviegalaxies | 14 | 19 | No | [§] |
| `moviegalaxies/pulp_fiction` | moviegalaxies | 38 | 102 | No | [§] |
| `moviegalaxies/rear_window` | moviegalaxies | 12 | 17 | No | [§] |
| `moviegalaxies/scarface` | moviegalaxies | 49 | 157 | No | [§] |
| `moviegalaxies/schindler_s_list` | moviegalaxies | 45 | 76 | No | [§] |
| `moviegalaxies/se7en` | moviegalaxies | 49 | 100 | No | [§] |
| `moviegalaxies/star_wars_episode_iv_a_new_hope` | moviegalaxies | 42 | 124 | No | [§] |
| `moviegalaxies/taxi_driver` | moviegalaxies | 22 | 57 | No | [§] |
| `moviegalaxies/the_big_lebowski` | moviegalaxies | 37 | 81 | No | [§] |
| `moviegalaxies/the_departed` | moviegalaxies | 51 | 117 | No | [§] |
| `moviegalaxies/the_godfather` | moviegalaxies | 42 | 104 | No | [§] |
| `moviegalaxies/the_lord_of_the_rings_the_fellowship_of_the_ring` | moviegalaxies | 24 | 106 | No | [§] |
| `moviegalaxies/the_matrix` | moviegalaxies | 31 | 88 | No | [§] |
| `moviegalaxies/the_shawshank_redemption` | moviegalaxies | 35 | 136 | No | [§] |
| `moviegalaxies/the_shining` | moviegalaxies | 21 | 48 | No | [§] |
| `moviegalaxies/the_silence_of_the_lambs` | moviegalaxies | 35 | 78 | No | [§] |
| `moviegalaxies/the_usual_suspects` | moviegalaxies | 35 | 130 | No | [§] |
| `moviegalaxies/titanic` | moviegalaxies | 70 | 299 | No | [§] |
| `moviegalaxies/toy_story` | moviegalaxies | 39 | 204 | No | [§] |
| `political/polblogs_full` | political | 1490 | 19025 | Yes | [‡] |
| `political/polblogs_subset` | political | 867 | 18280 | Yes | [‡] |
| `shakespeare/a_comedy_of_errors` | shakespeare | 20 | 130 | No | [‡] |
| `shakespeare/a_midsummer_nights_dream` | shakespeare | 30 | 238 | No | [‡] |
| `shakespeare/a_winters_tale` | shakespeare | 35 | 174 | No | [‡] |
| `shakespeare/alls_well_that_ends_well` | shakespeare | 24 | 112 | No | [‡] |
| `shakespeare/antony_and_cleopatra` | shakespeare | 54 | 313 | No | [‡] |
| `shakespeare/as_you_like_it` | shakespeare | 27 | 110 | No | [‡] |
| `shakespeare/coriolanus` | shakespeare | 61 | 429 | No | [‡] |
| `shakespeare/cymbeline` | shakespeare | 39 | 200 | No | [‡] |
| `shakespeare/hamlet` | shakespeare | 34 | 207 | No | [‡] |
| `shakespeare/henry_iv` | shakespeare | 35 | 152 | No | [‡] |
| `shakespeare/henry_v` | shakespeare | 47 | 228 | No | [‡] |
| `shakespeare/henry_vi_part_1` | shakespeare | 52 | 314 | No | [‡] |
| `shakespeare/henry_vi_part_2` | shakespeare | 64 | 422 | No | [‡] |
| `shakespeare/henry_vi_part_3` | shakespeare | 46 | 272 | No | [‡] |
| `shakespeare/henry_viii` | shakespeare | 46 | 212 | No | [‡] |
| `shakespeare/julius_caesar` | shakespeare | 50 | 290 | No | [‡] |
| `shakespeare/king_john` | shakespeare | 29 | 161 | No | [‡] |
| `shakespeare/king_lear` | shakespeare | 26 | 161 | No | [‡] |
| `shakespeare/loves_labours_lost` | shakespeare | 20 | 143 | No | [‡] |
| `shakespeare/macbeth` | shakespeare | 41 | 188 | No | [‡] |
| `shakespeare/measure_for_measure` | shakespeare | 25 | 110 | No | [‡] |
| `shakespeare/merchant_of_venice` | shakespeare | 23 | 119 | No | [‡] |
| `shakespeare/merry_wives_of_windsor` | shakespeare | 24 | 182 | No | [‡] |
| `shakespeare/much_ado_about_nothing` | shakespeare | 24 | 140 | No | [‡] |
| `shakespeare/othello` | shakespeare | 27 | 172 | No | [‡] |
| `shakespeare/pericles` | shakespeare | 46 | 185 | No | [‡] |
| `shakespeare/richard_ii` | shakespeare | 35 | 170 | No | [‡] |
| `shakespeare/richard_iii` | shakespeare | 68 | 477 | No | [‡] |
| `shakespeare/romeo_and_juliet` | shakespeare | 34 | 233 | No | [‡] |
| `shakespeare/taming_of_the_shrew` | shakespeare | 37 | 226 | No | [‡] |
| `shakespeare/the_tempest` | shakespeare | 20 | 121 | No | [‡] |
| `shakespeare/timon_of_athens` | shakespeare | 55 | 352 | No | [‡] |
| `shakespeare/titus_andronicus` | shakespeare | 27 | 179 | No | [‡] |
| `shakespeare/troilus_and_cressida` | shakespeare | 28 | 160 | No | [‡] |
| `shakespeare/twelfth_night` | shakespeare | 18 | 101 | No | [‡] |
| `shakespeare/two_gentlemen_of_verona` | shakespeare | 17 | 55 | No | [‡] |
| `social/dolphins_2` | social | 62 | 159 | No | [†] |
| `social/got_season1` | social | 127 | 550 | No | [‡] |
| `social/got_season2` | social | 129 | 486 | No | [‡] |
| `social/got_season3` | social | 124 | 504 | No | [‡] |
| `social/got_season4` | social | 172 | 667 | No | [‡] |
| `social/got_season5` | social | 119 | 398 | No | [‡] |
| `social/got_season6` | social | 143 | 542 | No | [‡] |
| `social/got_season7` | social | 81 | 412 | No | [‡] |
| `social/greys` | social | 54 | 57 | No | [†] |
| `social/highschool_boys` | social | 70 | 506 | Yes | [‡] |
| `social/karate` | social | 34 | 78 | No | [†] |
| `social/miserables` | social | 77 | 254 | No | [†] |
| `social/polbooks` | social | 105 | 441 | Yes | [†] |
| `sociology/coleman` | sociology | 73 | 263 | Yes | [†] |
| `sociology/eies_relations` | sociology | 32 | 768 | Yes | [‡] |
| `sociology/law_friends` | sociology | 71 | 575 | Yes | [‡] |
| `sociology/radoslaw_email` | sociology | 167 | 5784 | Yes | [‡] |
| `starwars/starwars_ep1` | starwars | 38 | 135 | No | [‡] |
| `starwars/starwars_ep2` | starwars | 33 | 101 | No | [‡] |
| `starwars/starwars_ep3` | starwars | 24 | 65 | No | [‡] |
| `starwars/starwars_ep4` | starwars | 21 | 60 | No | [‡] |
| `starwars/starwars_ep5` | starwars | 21 | 55 | No | [‡] |
| `starwars/starwars_ep6` | starwars | 20 | 55 | No | [‡] |
| `starwars/starwars_ep7` | starwars | 27 | 92 | No | [‡] |

> **[†]** Individual network citations listed in the References section below.
> **[‡]** Dataset sourced from the networkdata R package (Schoch 2020).
> **[§]** Dataset sourced from the MovieGalaxies project (Harvard Dataverse).

## References

- Coleman, J. S., Katz, E., & Menzel, H. (1957). The diffusion of an innovation among physicians. *Sociometry*, 20(4), 253–270.
- Grunspan, D. Z., et al. (2014). Understanding classrooms through social network analysis. *CBE Life Sciences Education*, 13(2), 167–178.
- Knuth, D. E. (1993). *The Stanford GraphBase: A Platform for Combinatorial Computing*. Addison-Wesley.
- Krebs, V. (2004). Political books network. Unpublished dataset, cited in Newman, M. E. J. (2006). Modularity and community structure in networks. *PNAS*, 103(23), 8577–8582.
- Lusseau, D., et al. (2003). The bottlenose dolphin community of Doubtful Sound features a large proportion of long-lasting associations. *Behavioral Ecology and Sociobiology*, 54(4), 396–405.
- Mersch, D. P., et al. (2013). Tracking individuals shows spatial fidelity is a key regulator of ant social organization. *Science*, 340(6136), 1090–1093.
- Young, S. J., & Scannell, J. W. (1993). Macaque cerebral cortex connectivity data. Cited in Schoch, D. (2020). networkdata: Repository of Network Datasets. R package.
- Zachary, W. W. (1977). An information flow model for conflict and fission in small groups. *Journal of Anthropological Research*, 33(4), 452–473.
- Schoch, D. (2020). networkdata: Repository of Network Datasets. R package version 0.1.12. https://CRAN.R-project.org/package=networkdata
- Gabasova, E. (2016). *Star Wars social network*. DOI: 10.5281/zenodo.1411479. Movie co-appearance networks from the Moviegalaxies project.
- Kaminski, J., Schober, M., Albaladejo, R., Zastupailo, O., & Hidalgo, C. (2018). *Moviegalaxies - Social Networks in Movies*. Harvard Dataverse. https://doi.org/10.7910/DVN/T4HBA3

---

*Datasets are provided for educational use. Please cite the original sources when using these networks in research publications.*
