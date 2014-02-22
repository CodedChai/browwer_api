browwer_api
===========



        var goodPositionChange = function(pos) {
          var crd = pos.coords;

          currentLatlng = [crd.latitude, crd.longitude];
          
        }
        
        
        badPositionChange = function (err) {
          console.warn('ERROR(' + err.code + '): ' + err.message);
        },
        options = {
          enableHighAccuracy: true,
        };
        
        
var positionWatchID = positionWatchID || navigator.geolocation.watchPosition(goodPositionChange, badPositionChange, options);
    
});


