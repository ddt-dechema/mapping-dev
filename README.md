# Changelog
### 2020-Jan-27
* Corrected calculation for minimal CO availability.
 In main.js the function *decideIfInVisibleCluster* used to contain a old (?) value for the minimal CO availability (15 kt instead of 13.5 kt)

### 2020-Feb-07
* Updated the corrected data for plant "ArcelorMittal Bremen GmbH", due to data on E-PRTR website being wrong (noticed by FA).
* running *sparql.html*, subsequently updated *prtr.json*, as well as re-running *chemicalParkDistances.html* and lastly updating *emissions.json*

# mapping
The mapping activities from the Carbon4PUR project.

This fork's site (by ddt-dechema) can be visited via https://ddt-dechema.github.io/mapping-dev/

# Workflow
## Emissions
Open sparql.html and wait for it to complete. The result will be logged in the console. Copy the object and paste it in prtr.json.
Careful: we corrected the coordinates for one plant (see comment in top of file), please keep those changes in the new version.
Attention: Don't forget to run chemicalParkDistances.html (see chapter "distances" below)

## Chemical parks and polyol plants
The list of all chemical plants known to us is in chemicalparks.csv, all polyol plants are in "polyol plants europe v2.csv".

Both can be converted by opening chemParksConverter.html. The last result object in the console can be copied to "chemicalParks.json.

## Distances

By running chemicalParkDistances.html, chemicalParks.json and prtr.json will be loaded and distances added to the emissions data. Copy the resulting object into "emissions.json".

Done, you have a working version with updated data.

# Disclaimer
![EU logo](img/eu.png "EU logo")
This project has received funding from the European Union's Horizon 2020 research and innovation programme under grant agreement No 768919

The information contained in this document has been prepared solely for the purpose of providing information about the Carbon4PUR consortium and its project. The document reflects only the Carbon4PUR consortium’s view and the European Commission is not responsible for any use that may be made of the information it contains.

# License
The content of this site is licensed under the <a href="https://opensource.org/licenses/MIT">MIT	license</a>. You are basically free to do anything you want with it as long as you cite the authour	(Carbon4PUR consortium) and use a similarly permissive license.
Please feel free to clone, modify and create pull requests. 
