CASSANDRE - Texts archive for qualitative analysis
==================================================

License: [GNU Affero General Public License](http://www.gnu.org/licenses/agpl.html)

Contact: <christophe.lejeune@ulg.ac.be>

Home page: <https://github.com/Hypertopic/Cassandre>

Notice
------

Cassandre is a server software. There is no need to install it on your own computer to use it. The usual way is to be "hosted" by one's own institution (ask your system administrator). If your use cases meet our research interests, we can also host your data on our community server.

Installation requirements
-------------------------

* Git client
* [CouchDB](http://couchdb.apache.org/)
* [CouchApp](https://github.com/jchris/couchapp) 
* [Node.js](http://nodejs.org/)

Installation procedure
----------------------

* Create a database named ``cassandre`` at <http://127.0.0.1:5984/_utils>.

* In any folder:

        git clone https://github.com/Hypertopic/Cassandre.git
        cd Cassandre
        couchapp init
        couchapp push http://127.0.0.1:5984/cassandre
        cd node
        npm install express
        npm install express-http-proxy
        npm install async

* Change settings in `app.js`.
* Test the settings (`sudo` is required for port 80):

        sudo node app.js
