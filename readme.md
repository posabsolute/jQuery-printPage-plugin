#jQuery printPage plugin

Print any page within your website without quitting your page.

Typically you would create a special print template, open it in a popup and then call window.print().This plugin take the page you want to print, put it in an iframe and print it without the need of a popup

Also, because you still actually link to your popup, if some of your users have javascript disabled, they could still open the special template and print it.

Example: http://www.position-absolute.com/creation/print/

##Using it

    $(".btnPrint").printPage()

##Optional
There is some options available:
###url: Overwrite the automatic url fetching in the href attribute
###message: The text message displayed before the print page is loaded
###attr (default: href) : change the default href attribute that is used to retrieve the print page URL.


    $(".btnPrint").printPage({
      url: "/print/custompage/html",
      attr: "href",
      message:"Your document is being created"
    })

To be a little more specific, if you declare a url it will not look in the attribut and directly use this one.

##Tested on:
Firefox 3.6
IE 7&8
Chrome latest

** I use a data url background image and some CSS3 properties for the little warning box, you might want to have a look if you care about IE

[![endorse](http://api.coderwall.com/posabsolute/endorsecount.png)](http://coderwall.com/posabsolute)