<script>
let hp = 25;
let ac = 20;
let tempHP = 5;
let speed = 35;
let initiative = 3;
</script>


<div class="table-container mt-3 mb-2">
	<table class="table table-hover variant-ghost-primary">
		<thead class="variant-ghost-secondary">
			<tr>
				<th class="text-center">Hit points</th>
				<th class="text-center">Armor Class</th>
                <th class="text-center">Temporary HP</th>
                <th class="text-center">Speed</th>
			</tr>
		</thead>
		<tbody>
				<tr class="text-center">
					<td>{hp}</td>
					<td>{ac}</td>
                    <td>{tempHP}</td>
                    <td>{speed}</td>
				</tr>
		</tbody>
	
	</table>
</div>



