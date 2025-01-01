# ed-colonisation-planner
A colonisation planner for Elite: Dangerous

There's no specific goal for this project. It'll likely just be a collection of personal-use scripts for
various tasks relating to the upcoming colonisation feature in Elite. The features/scripts are listed below.
The same information can also be found at the top of each script file.

## Unpopulated ELW Finder
This script finds unpopulated systems with Earth-like Worlds (ELWs) within a given radius of a specified system.
The minimum and maximum radius are configurable, as well as the origin system.

Because the EDSM API is limited in the functionality it exposes, this script first gets all systems in the radius and
then filters down to unpopulated systems with ELWs. Because of this approach, the script may take a long time to run
if the search radius is large.
