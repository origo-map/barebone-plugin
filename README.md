# Barebone plugin

This is just an example plugin

#### Example usage of Barebone plugin

**index.html:**
```
    <head>
    	<meta charset="utf-8">
    	<meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
    	<meta http-equiv="X-UA-Compatible" content="IE=Edge;chrome=1">
    	<title>Origo exempel</title>
    	<link href="css/style.css" rel="stylesheet">
    	<link href="plugins/barebone.css" rel="stylesheet">
    </head>
    <body>
    <div id="app-wrapper">
    </div>
    <script src="js/origo.js"></script>
    <script src="plugins/barebone.js"></script>

    <script type="text/javascript">
      //Init origo
      var origo = Origo('index.json');
      origo.on('load', function (viewer) {
        var barebone = Barebone({
          buttonText: 'Click this!',
          content: 'Just nonsense'
        });
        viewer.addComponent(barebone);
      });
    </script>
```
 Codepen: https://codepen.io/jokd/pen/VwmgjYP
