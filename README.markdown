PyXMLi helps Python developers generate invoices in [XMLi 2.0](http://www.xmli.org), the open-source invoice format designed by [Greendizer](http://greendizer.com).

##Why another format?
Simply because none of the available formats was good enough for what its creators needed it for.

##Design goals
-    Human-readable, *Web-friendly* format; 
-    Carry data structures, not business logic;
-    Stand-alone, with every detail possible from creation to archiving;
-    Privilege existing standards whenever possible.

##Features
PyXMLi comes with a great deal of features to make it really easier for Python developers to:

-    Generate XMLi 2.0 invoices in their favorite language;
-    Strongly validate pretty much every field locally before sending their invoices; 
-    Sign their invoices using the XMLDsig standard and a simple RSA key.

##Requirements
-    Python 2.5+
-    lxml 2.3+
-    pyCrypto 2.6+

(Built-in setup will install all the dependencies automatically).

##Compatibility
PyXMLi is compatible with Google App Engine and their Python 2.7 runtime.

Edit app.yaml to add pyCrypto and lxml to the list of third-party modules you'd like to use. 

    libraries:
    - name: pycrypto
      version: 2.6
    
    - name: lxml
      version: 2.3

##Setup
Using *pip*:

    sudo pip install --upgrade pyxmli

Using *easy_install*:

    sudo easy_install --upgrade pyxmli
    
Using source code:

    sudo python setup.py install