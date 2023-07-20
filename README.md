# init_v2
jQuery JavaScript initialize v2  module and plugin development

```JS
   const v2nielsOffice = (function() {

    let visibilityBy = 9999999;
    let cIndex = 0;
     
    const currentIndex = function( cIndex = {} ) { this.currentIndex = cIndex }
    // const findChild = function( fChild = {} ) { this.findChildren = fChild } 

    const checkCurrentIndex = function( $obj ) {

      currentIndex.prototype.init = function() {

        let ic  = this.currentIndex;
        let ciD = ic.pID;
        currentIndex.prototype.layout(ciD);

      }
      currentIndex.prototype.layout = function( obj ) {
          console.log( visibilityBy );
          console.log( obj );
      }

      return new currentIndex( $obj ).init();

    };

    /*
    const checkCurrentChild = function( $obj ) {

      findChild.prototype.init = function() {

        let ic  = this.currentIndex;
        let ciD = ic.pID;
        currentIndex.prototype.layout(ciD);

      }
      findChild.prototype.layout = function( obj ) {
   
      }

      return new findChild( $obj ).init();

    } */
    
    // Init method
    const initialize = function( init = {} ) {
    
      checkCurrentIndex(init);
  /*  checkCurrentChild(init); */

    }

    return { 
      
      init : initialize
  
    }
   })();

   if( typeof v2nielsOffice === 'object') {
    v2nielsOffice.init({
      pID : '#parentContainer'

    });
   }

```
