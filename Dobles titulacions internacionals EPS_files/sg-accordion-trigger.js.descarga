/*
 Saga Suite Accordion Trigger:
  Cambia el icono de despliegue o pliegue en cualquier accordionde bootstrap
*/
$(document).ready(function () {

	$('.panel-group').on('shown.bs.collapse', function (e) {
		$(e.target).parent().find('a[aria-expanded="true"] .fa-angle-down').removeClass('fa-angle-down').addClass('fa-angle-up');
	});
	$('.panel-group').on('show.bs.collapse', function (e) {
		$(e.currentTarget).find('open').removeClass('open');
		$(e.target).parent().addClass('open');
	});

	$('.panel-group').on('hidden.bs.collapse', function (e) {
		$(e.target).parent().find('a[aria-expanded="false"] .fa-angle-up').removeClass('fa-angle-up').addClass('fa-angle-down');
	});
	$('.panel-group').on('hide.bs.collapse', function (e) {
		$(e.target).parent().removeClass('open');
	});
	
});