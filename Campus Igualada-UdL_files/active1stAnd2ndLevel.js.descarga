$(document).ready(function () {
    var path = window.location.pathname;
    path = path.replace(/\/$/, "");
    path = decodeURIComponent(path);

    $(".mega-menu .nav a").each(function(){
        var href = $(this).attr('href');
        href = href.replace(/\/$/, "");
        href = decodeURIComponent(href);
        if (path.substring(0, href.length) === href) {
            $(this).closest('li').addClass('active');
            $(this).closest('ul').prev('.h3').addClass('active');

            var parent = $(this).parents('li.mainnav-lvl1.dropdown');
            var parentHref = parent.find('a.mainnav-lvl1.dropdown-toggle').attr("href");
            if (parentHref) {
                parentHref = parentHref.replace(/\/$/, "");
                parentHref = decodeURIComponent(parentHref);

                if (path.substring(0, parentHref.length) === parentHref) {
                    parent.addClass("active");

                }
            }
        }
    });
});