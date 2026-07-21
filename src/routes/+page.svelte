<script>
    import { DateTime } from "luxon";
	var schedule = {
		className: 'X-3',
		school: 'Sekolah Citra Kasih Don Bosco Pondok Indah',
		academicYear: '2026-2027',
		semester: 1,
		term: 1,
		notes: [
			'ICTC pada minggu 1 & 3 sesuai jadwal',
			'BK pada minggu 2 & 4 sesuai jadwal',
			'FUTURE GATE dimulai minggu ke-3 Agustus'
		],
		schedule: {
			Monday: [
				{ time: '07:00-07:15', period: 0, subject: 'Morning Devotion', teacher: '' },
				{ time: '07:15-08:00', period: 1, subject: 'ICTC / BK', teacher: 'Mr. Andika / Ms. Fiona' },
				{ time: '08:00-08:45', period: 2, subject: 'ICTC / BK', teacher: 'Mr. Andika / Ms. Fiona' },
				{ time: '08:45-09:30', period: 3, subject: 'Bahasa Inggris', teacher: 'Mr. Juan' },
				{ time: '09:30-09:45', period: null, subject: 'Break', teacher: '' },
				{ time: '09:45-10:25', period: 4, subject: 'Ekonomi', teacher: 'Ms. Rina' },
				{ time: '10:25-11:05', period: 5, subject: 'PoE', teacher: 'Mr. Aldrich' },
				{ time: '11:05-11:45', period: 6, subject: 'PoE', teacher: 'Mr. Aldrich' },
				{ time: '11:45-12:25', period: 7, subject: 'Pendidikan Agama', teacher: 'Ms. Tiara' },
				{ time: '12:25-12:55', period: null, subject: 'Lunch Break', teacher: '' },
				{ time: '12:55-13:35', period: 8, subject: 'Pendidikan Agama', teacher: 'Ms. Tiara' },
				{ time: '13:35-14:15', period: 9, subject: 'Geografi', teacher: 'Ms. Lia' },
				{ time: '14:15-14:55', period: 10, subject: 'Geografi', teacher: 'Ms. Lia' },
				{ time: '14:55-15:10', period: null, subject: 'Dismissal', teacher: '' }
			],
			Tuesday: [
				{ time: '07:00-07:15', period: 0, subject: 'Morning Devotion', teacher: '' },
				{ time: '07:15-08:00', period: 1, subject: 'Bahasa Indonesia', teacher: 'Ms. Angelina' },
				{ time: '08:00-08:45', period: 2, subject: 'Bahasa Indonesia', teacher: 'Ms. Angelina' },
				{ time: '08:45-09:30', period: 3, subject: 'Biologi', teacher: 'Ms. Ely' },
				{ time: '09:30-09:45', period: null, subject: 'Break', teacher: '' },
				{ time: '09:45-10:25', period: 4, subject: 'Sejarah', teacher: 'Mr. Ian' },
				{ time: '10:25-11:05', period: 5, subject: 'Sejarah', teacher: 'Mr. Ian' },
				{ time: '11:05-11:45', period: 6, subject: 'Penjasorkes', teacher: 'Mr. Andreas' },
				{ time: '11:45-12:25', period: 7, subject: 'Penjasorkes', teacher: 'Mr. Andreas' },
				{ time: '12:25-12:55', period: null, subject: 'Lunch Break', teacher: '' },
				{ time: '12:55-13:35', period: 8, subject: 'Sosiologi', teacher: 'Mr. John' },
				{ time: '13:35-14:15', period: 9, subject: 'Sosiologi', teacher: 'Mr. John' },
				{ time: '14:15-14:55', period: 10, subject: 'Kimia', teacher: 'Ms. Aurellia' },
				{ time: '14:55-15:35', period: 11, subject: 'Kimia', teacher: 'Ms. Aurellia' }
			],
			Wednesday: [
				{ time: '07:00-07:15', period: 0, subject: 'Morning Devotion', teacher: '' },
				{
					time: '07:15-08:00',
					period: 1,
					subject: 'Seni Budaya',
					teacher: 'Ms. Anne / Mr. Michael / Mr. Prima'
				},
				{
					time: '08:00-08:45',
					period: 2,
					subject: 'Seni Budaya',
					teacher: 'Ms. Anne / Mr. Michael / Mr. Prima'
				},
				{ time: '08:45-09:30', period: 3, subject: 'Ekonomi', teacher: 'Ms. Rina' },
				{ time: '09:30-09:45', period: null, subject: 'Break', teacher: '' },
				{ time: '09:45-10:25', period: 4, subject: 'Ekonomi', teacher: 'Ms. Rina' },
				{ time: '10:25-11:05', period: 5, subject: 'Bahasa Inggris', teacher: 'Mr. Juan' },
				{ time: '11:05-11:45', period: 6, subject: 'Bahasa Inggris', teacher: 'Mr. Juan' },
				{ time: '11:45-12:25', period: 7, subject: 'Bahasa Inggris', teacher: 'Mr. Juan' },
				{ time: '12:25-12:55', period: null, subject: 'Lunch Break', teacher: '' },
				{ time: '12:55-13:35', period: 8, subject: 'Bahasa Indonesia', teacher: 'Ms. Angelina' },
				{ time: '13:35-14:15', period: 9, subject: 'Bahasa Indonesia', teacher: 'Ms. Angelina' },
				{ time: '14:15-14:55', period: 10, subject: 'PPals', teacher: 'Mentor' },
				{ time: '14:55-15:35', period: 11, subject: 'PPals', teacher: 'Mentor' }
			],
			Thursday: [
				{ time: '07:00-07:15', period: 0, subject: 'Morning Devotion', teacher: '' },
				{ time: '07:15-08:00', period: 1, subject: 'Informatika', teacher: 'Ms. Mei' },
				{ time: '08:00-08:45', period: 2, subject: 'Informatika', teacher: 'Ms. Mei' },
				{ time: '08:45-09:30', period: 3, subject: 'Fisika', teacher: 'Ms. Suida' },
				{ time: '09:30-09:45', period: null, subject: 'Break', teacher: '' },
				{ time: '09:45-10:25', period: 4, subject: 'Matematika', teacher: 'Ms. Yustina' },
				{ time: '10:25-11:05', period: 5, subject: 'Matematika', teacher: 'Ms. Yustina' },
				{ time: '11:05-11:45', period: 6, subject: 'Mandarin', teacher: 'Ms. Egy' },
				{ time: '11:45-12:25', period: 7, subject: 'Mandarin', teacher: 'Ms. Egy' },
				{ time: '12:25-12:55', period: null, subject: 'Lunch Break', teacher: '' },
				{ time: '12:55-13:35', period: 8, subject: 'Kimia', teacher: 'Ms. Aurellia' },
				{ time: '13:35-14:15', period: 9, subject: 'Pendidikan Pancasila', teacher: 'Mr. John' },
				{ time: '14:15-14:55', period: 10, subject: 'Pendidikan Pancasila', teacher: 'Mr. John' },
				{ time: '14:55-15:10', period: null, subject: 'Dismissal', teacher: '' }
			],
			Friday: [
				{ time: '07:00-07:15', period: 0, subject: 'Morning Devotion', teacher: '' },
				{ time: '07:15-07:55', period: 1, subject: 'Matematika', teacher: 'Ms. Yustina' },
				{ time: '07:55-08:35', period: 2, subject: 'Matematika', teacher: 'Ms. Yustina' },
				{ time: '08:35-09:15', period: 3, subject: 'Biologi', teacher: 'Ms. Ely' },
				{ time: '09:15-09:30', period: null, subject: 'Break', teacher: '' },
				{ time: '09:30-10:10', period: 4, subject: 'Biologi', teacher: 'Ms. Ely' },
				{ time: '10:10-10:50', period: 5, subject: 'Fisika', teacher: 'Ms. Suida' },
				{ time: '10:50-11:30', period: 6, subject: 'Fisika', teacher: 'Ms. Suida' },
				{ time: '11:30-12:10', period: 7, subject: 'CT Time / Fellowship', teacher: '' },
				{ time: '12:10-13:00', period: null, subject: 'Lunch Break', teacher: '' },
				{ time: '13:00-14:30', period: null, subject: 'FUTURE GATE', teacher: '' }
			]
		}
	};
    var dt = DateTime.now();
    var day = $state(dt.toLocaleString({weekday: 'long'}));
    var tommorow = $state(dt.plus({days: 1}).toLocaleString({weekday: 'long'}));
    var colors = {
        "Morning Devotion": "text-purple-600",
        "ICTC / BK": "text-sky-600",
        "Bahasa Inggris": "text-amber-600",
        "Bahasa Indonesia": "text-yellow-600",
        "Mandarin": "text-orange-600",
        "Matematika": "text-blue-600",
        "Biologi": "text-emerald-600",
        "Fisika": "text-cyan-600",
        "Kimia": "text-teal-600",
        "Ekonomi": "text-lime-600",
        "Geografi": "text-green-600",
        "Sejarah": "text-stone-600",
        "Sosiologi": "text-rose-600",
        "Pendidikan Agama": "text-violet-600",
        "Pendidikan Pancasila": "text-red-600",
        "Penjasorkes": "text-indigo-600",
        "Seni Budaya": "text-fuchsia-600",
        "Informatika": "text-indigo-600",
        "PoE": "text-pink-600",
        "PPals": "text-purple-600",
        "CT Time / Fellowship": "text-indigo-600",
        "FUTURE GATE": "text-blue-700",
        "Break": "text-gray-400",
        "Lunch Break": "text-gray-400",
        "Dismissal": "text-gray-400"
    }
</script>
<div class="ml-auto flex gap-y-1 text-zinc-500 text-sm absolute top-10 left-3 flex-col">
    <h3 class="font-bold">Today's schedule ({day})</h3>
    {#each schedule.schedule[day] as subject}
        <p class="font-medium {colors[subject.subject]}">{subject.subject} <span class="text-zinc-800 font-semibold">({subject.time})</span></p>
    {/each}
</div>
<div class="ml-auto flex gap-y-1 text-zinc-500 text-sm absolute top-10 right-3 flex-col text-right">
    <h3 class="font-bold">Tommorow's schedule ({tommorow})</h3>
    {#each schedule.schedule[tommorow] as subject}
        <p class="font-medium {colors[subject.subject]}">{subject.subject} <span class="text-zinc-800 font-semibold">({subject.time})</span></p>
    {/each}
</div>
<div class="flex h-full flex-col">
	<div class="bg-green-300 p-1 px-3 flex">
		<h1 class="text-green-900 font-black">X-3 Dashboard</h1>
	</div>
	<div
		class="flex h-full flex-col items-center justify-center gap-y-6 text-center text-2xl font-black"
	>
		<a href="https://treasury.vostro.my.id" class="duration-200 hover:text-3xl hover:text-zinc-500"
			>Treasury (WIP)</a
		>
		<a
			href="https://drive.google.com/file/d/1iLih0vA7ohqIrwDx13f3QOaZh-hn-ZHZ/view?usp=sharing"
			class="duration-200 hover:text-3xl hover:text-zinc-500">Weekly Agenda</a
		>
	</div>
</div>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Quicksand:wght@300..700&display=swap');
	* {
		font-family: Quicksand;
	}
	:global(html, body) {
		height: 100%;
	}
</style>
