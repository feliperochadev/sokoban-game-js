Credits to bogar (https://github.com/borgar/jquery-sokoban)

# Sōkoban Game

An Adaptation of implementation of Bogar Sokōban in JavaScript, as a [jQuery] plugin. 
## How to use

1. Include a reference to the plugin (and jQuery) to the `<head>` section of your document:

        <script src="jquery.min.js"></script>
        <script src="jquery.sokoban.js"></script>


2. Add a Sokoban puzzle to your HTML document:

        <pre class="sokoban>
        ####
        # .#
        #  ###
        #*@  #
        #  $ #
        #  ###
        ####
        </pre>

3. Run the game when the document loads:

        <script>
        jQuery(function($){
          $('pre.sokoban').sokoban();
        });
        </script>

        optional parameters are: 
        -originalLevels: (Array) to get all text original levels
        -reset: (bool) to only reset the level dont create a new one
        -level: (int) get the current level to reset

        eg: $('pre.sokoban').sokoban(originalLevels, reset, level);



  [jQuery]: http://jquery.com/

4. Consider adding CSS styles to make the levels look nicer (some are included in the project).
