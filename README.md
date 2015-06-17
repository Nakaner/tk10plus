tk10plus
========

tk10plus is a collection of rendering styles which 
look like a German "Topographische Karte 1:10.000" 
(topographical map 1:10,000) but contains a little bit 
more information.

License
=======
see LICENSE.md
Please remember that usage of OSM data has to be attributed! See https://osm.org/copyright for further details. 


Maperitive
==========
Setup
-----
1. Create a link from your Maperitive icons directory to tk10plus/icons/michreichert. On Linux/OS X run following command from the directory where Maperitive is installed:
    cd icons && ln -s <path to tk10plus repository>/icons/michreichert michreichert
2. In Maperitive: 
    use-ruleset location=<path to tk10plus repository>/tk10plus/tk10better.mrules as-alias=tk10better
3. In Maperitive: Map -> Switch to Rules -> tk10better
4. Load Conture Lines: Tools -> Generate Relief Contures


Mapserver
=========
Dependencies
------------
* Mapserver 6.0 or newer
* Imposm
* PostGIS 2.1 (maybe also 2.0 but not tested) with legacy.sql enabled
* OSM data has to be imported using imposm 2 using this scheme: https://bitbucket.org/olt/imposm/src/tip/imposm/defaultmapping.py

Notes
-----
This style is a development preview. It lacks all icons, most labels, multi-colour textures  (e.g. wetland) and conture lines.