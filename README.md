ColReorderWithResize
====================

Column reordering with resizable columns plug-in for DataTables

New options include:

minResizeWidth: (default: 10). Minimum size that columns can be.

bResizeTable: (Default: true). Allow table to be resized. Column resize events will grow or shrink table

bAddFixed: (default: true). Automtically add taable-layout:fixed CSS to a table

fnResizeTableCallback: Call function every time the table is resized

allowResize (default: true): Allow table to be resized

allowHeaderDoubleClick (default: true): Double-clicking on header field will expand to "full size". double-clicking again will reduce to minimum size.

Other options remain the same as those in the <a href="http://datatables.net/extras/colreorder/">ColReorder</a> plugin.

Basic initialization:
`````javascript
$(document).ready( function () {
    $('#example').dataTable( {
        "sDom": 'Rlfrtip'
    } );
} );
`````

The "R" option in sDom enables this feature.

Additional options can be set with "oColReorder":
`````javascript
$(document).ready( function () {
    $('#example').dataTable( {
        "sDom": 'Rlfrtip',
        "oColReorder": {
            "bAddFixed":false
        }
    } );
} );
`````
