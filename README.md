# Einleitung
Dies ist ein Repository, welches für eine Abschlussarbeit zu dem Thema "Optimierung der Netzanschlusspunktauslastung von nachhaltigen Energieerzeugungsanlagen mit Schwerpunkt auf Kombination von Photovoltaik, Windkraft und Batteriespeicher" erstellt wurde. Die Bereitstellung des Repositorys erfolgt aus Gründen der Transparenz und Nachvollziehbarkeit. 

# Beschreibung der verwendeten Datein
Die Ordner von Nord bis Zentrum enthalten zum einen die verwendete Datengrundlage der Wetterereignisse und zum anderen Metadaten für die Nachvollziehbarkeit der Messverfahren. Die Daten entstammen dem Deutschen Wetterdienst.

Die CSV-Datei "Spotmarktpreis [2015-2024].csv" enthält den verwendeten Verlauf der Spotmarktpreise am Day-Aheadmartk gemäß Netztransparenz.de. Diese muss bei Bedarf zur Anwendung über die unten stehende Quelle gedownloadet und wie beschrieben benannt werden. Alternativ kann in "model.ipynb" der einzulesende Name in Zelle 3 angepasst werden.

Die Jupyter-Notebook-Datein "model.ipynb" umfasst den gesamten Code und selbsterstellten Abbildungen, die in der Abschlussarbeit verwendet wurden.

"requirements.txt" dient zur Reproduzierbarkeit und listet die Python-Bibliotheken, die benötigt werden, um "model.ipynb" ausführen zu können. 

# Verwendung des Programms
Über GitHub können die zuletzt ausgeführten Zellen mit ihren Ergebnissen betrachtet werden. Falls darüber hinaus das Bedürfnis zur Verwendung des Programms entsteht, muss mindestens Python installiert sein. Über Pip von Python müssen die requirements installiert werden. Über eine IDE, die Jupyter Notebooks ausführen kann oder Jupyter Notebook selbst kann die Ausführung der Datei "model.ipynb" erfolgen. Der bereitgestellte Code muss angepasst werden, um andere Werte oder insbesondere andere Anlagenkonstellationen anzuzeigen oder zu berechnen.

# Quellen
## Verwendete Datensätze
### historische Wetterdaten (2020-2024) für die Anlagen mit den Stations-IDs: 00591, 01048, 05404, 03098, 03231

Deutscher Wetterdienst. (2024). 10-minütige Stationsmessungen der Lufttemperatur für Deutschland (Version v24.03). Abgerufen am 18. June 2025 von https://opendata.dwd.de/climate_environment/CDC/observations_germany/climate/10_minutes/air_temperature/

Deutscher Wetterdienst. (2024). 10-minütige Stationsmessungen der Strahlung und Sonnenscheindauer für Deutschland (Version v24.03). Abgerufen am 18. June 2025 von https://opendata.dwd.de/climate_environment/CDC/observations_germany/climate/10_minutes/solar/

Deutscher Wetterdienst. (2024). 10-minütige Stationsmessungen des Windes für Deutschland (Version v24.03). Abgerufen am 18. June 2025 von https://opendata.dwd.de/climate_environment/CDC/observations_germany/climate/10_minutes/wind/

lizenziert unter CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/).

### Spotmarktpreise (2015-2024)

Netztransparenz.de. (2025). Spotmarktpreis nach § 3 Nr. 42a EEG. Abgerufen am 2. July 2025 von https://www.netztransparenz.de/de-de/Erneuerbare-Energien-und-Umlagen/EEG/Transparenzanforderungen/Marktpr%C3%A4mie/Spotmarktpreis-nach-3-Nr-42a-EEG

## externe Python-Bibliotheken und Programme
### pandas:
McKinney, W. (2010). Data Structures for Statistical Computing in Python. In S. van der Walt, & J. Millman (Hrsg.), Proceedings of the 9th Python in Science Conference, (S. 56-61). https://doi.org/10.25080/Majora-92bf1922-00a  

### numpy:
Harris, C. R., Millman, K. J., van der Walt, S. J., Gommers, R., Virtanen, P., Cournapeau, D., Wieser, E., Taylor, J., Berg, S., Smith, N. J., Kern, R., Picus, M., Hoyer, S., van Kerkwijk, M. H., Brett, M., Haldane, A., del Río, J. F., Wiebe, M., Peterson, P., Gérard-Marchant, P., . . . Oliphant, T. E. (September 2020). Array programming with NumPy. Nature, 585, 357–362. https://doi.org/10.1038/s41586-020-2649-2  

### scipy:
Virtanen, P., Gommers, R., Oliphant, T. E., Haberland, M., Reddy, T., Cournapeau, D., Burovski, E., Peterson, P., Weckesser, W., Bright, J., van der Walt, S. J., Brett, M., Wilson, J., Millman, K. J., Mayorov, N., Nelson, A. R., Jones, E., Kern, R., Larson, E., Carey, C. J., . . . Contributors, S. 1. (2020). SciPy 1.0: Fundamental Algorithms for Scientific Computing in Python. Nature Methods, 17, 261–272. https://doi.org/10.1038/s41592-019-0686-2  

### matplotlib:
Hunter, J. D. (2007). Matplotlib: A 2D graphics environment. Computing in Science & Engineering, 9, 90–95. https://doi.org/10.1109/MCSE.2007.55  

### seaborn:
Waskom, M. L. (2021). seaborn: statistical data visualization. Journal of Open Source Software, 6, 3021. https://doi.org/10.21105/joss.03021  

### pvlib:
Anderson, K. S., Hansen, C. W., Holmgren, W. F., Jensen, A. R., Mikofski, M. A., & Driesse, A. (December 2023). pvlib python: 2023 project update. Journal of Open Source Software, 8, 5994. https://doi.org/10.21105/joss.05994  

### windpowerlib:
Sabine Haas, Uwe Krien, Birgit Schachler, Stickler Bot, Velibor Zeli, Florian Maurer, Kumar Shivam, Francesco Witte, Sasan Jacob Rasti, Seth, & Stephen Bosch. (2024). wind-python/windpowerlib: Update release. Zenodo. https://doi.org/10.5281/ZENODO.10685057  

### pyomo:
Bynum, M. L., Hackebeil, G. A., Hart, W. E., Laird, C. D., Nicholson, B. L., Siirola, J. D., Watson, J.-P., Woodruff, D. L., & others. (2021). Pyomo-optimization modeling in python (Bd. 67). Springer.  

### Gurobi:
Gurobi Optimization, LLC. (2024). Gurobi Optimizer Reference Manual. https://www.gurobi.com




