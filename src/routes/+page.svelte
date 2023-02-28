<script>
	import Calendar from '@event-calendar/core';
	import Interaction from '@event-calendar/interaction';
	import DayGrid from '@event-calendar/day-grid';
	import '@event-calendar/core/index.css';

	let plugins = [DayGrid, Interaction];
	let options = {
		view: 'dayGridMonth',
		events: [{ title: 'Mr Smith', start: '2023-03-20', end: '2023-03-25' }],
		eventColor: '#378006',
		dateClick: function (info) {
			console.log(info);
		}
	};
</script>

<h3>Availability "La Civettaia"</h3>

<Calendar {plugins} {options} />
