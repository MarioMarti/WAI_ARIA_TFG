// funcion para igualar el alto de cajas con la misma clase, igualando al alto mayor

jQuery.fn.equalHeights = function() {
    var maxHeight = 0;
    // get the maximum height
    this.each(function(){
        var $this = jQuery(this);
        if ($this.height() > maxHeight) { maxHeight = $this.height(); }
    });
    // set the elements height
    this.each(function(){
        var $this = jQuery(this);
        $this.height(maxHeight);
    });
};

jQuery(window).load(function() {
    var classes = ["equalheight","equalheight-two","equalheight-three","equalheight-four","equalheight-five"];
    for (var i = 0, j = classes.length; i < j; i++) {
        jQuery('.' + classes[i]).equalHeights();
    }
});