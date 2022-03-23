<script>
  import AudioPlayer from './AudioPlayer.svelte';
	
	let audioURL = ""
</script>

<section id="section-3" class="section-divider-ipg">
			<h3 class="heading-2-ipg">Section Three</h3>
			<h3 class="heading-3-ipg">Pāli-alphabet</h3>
			<p class="paragraph-1-ipg">
				It is said that <span class="italic-w-ipg">Pāli</span> was a <a href="#section3-note-9" class="notes-ipg" id="section3-note-9-rtn"><span class="italic-w-ipg">vernacular</span><sup class="sup-spacing-ipg">9</sup></a> of northern India in the time of Gotama the Buddha. In India the alphabet has been preserved in the Devānagarī script, various other countries developed different other characters to express the <span class="italic-w-ipg">Pāli</span>language. To make it transferable into Roman script the following set of diacritical marks has been established to indicate the proper pronunciation.
			</p>

			<p class="paragraph-1-ipg">
				The alphabet consists of forty-one characters:  eight vowels and thirty-three consonants.
			</p>

			<p class="paragraph-2-ipg">The Vowels:</p>
			<div class="responsive-table-ipg">
				<!-- table-1 left-data, right-data-->
				<table class="vowel-list-ipg table-regular-ipg">
					<tbody><tr>
						<td><span class="italic-w-ipg">a</span></td>
						<td><span class="italic-w-ipg">ā</span></td>
					</tr>
					<tr>
						<td><span class="italic-w-ipg">i</span></td>
						<td><span class="italic-w-ipg">ī</span></td>
					</tr>
					<tr>
						<td><span class="italic-w-ipg">u</span></td>
						<td><span class="italic-w-ipg">ū</span></td>
					</tr>
					<tr>
						<td><span class="italic-w-ipg">e</span></td>
						<td><span class="italic-w-ipg">o</span></td>
					</tr>
				</tbody>
				</table>
			</div>

			<p class="paragraph-1-ipg">
				Vowels can be short and long; a line over a vowel - ā, ī, ū - indicates a long vowel that resonates for about twice the time period of a short <a href="#section3-note-10" class="notes-ipg" id="section3-note-10-rtn"><span class="italic-w-ipg">vowel</span><sup class="sup-spacing-ipg">10</sup></a>.  As far as similarity to English is concerned the following pronunciation aid may be <a href="#section3-note-11" class="notes-ipg" id="section3-note-11-rtn"><span class="italic-w-ipg">helpful</span><sup class="sup-spacing-ipg">11</sup></a>:
			</p>
			<div class="responsive-table-ipg">
				<!-- table-1 left-data, right-data-->
				<table class="vowel-list-ipg table-regular-ipg">
					<tbody><tr>
						<td><span class="italic-w-ipg">a</span> - as the "a" in cut</td>
						<td><span class="italic-w-ipg">ā</span> - as the "a" in art</td>
					</tr>
					<tr>
						<td><span class="italic-w-ipg">i</span> - as the "i" in mint</td>
						<td><span class="italic-w-ipg">ī</span> - as the "ee" in see  </td>
					</tr>
					<tr>
						<td><span class="italic-w-ipg">u</span> - as the "u" in put </td>
						<td><span class="italic-w-ipg">ū</span> - as the "oo" in cool</td>
					</tr>
				</tbody>
				</table>
			</div>

			<p class="paragraph-section3 reduce-mar-bottom-ipg"><span class="italic-w-ipg">-e-</span> and  <span class="italic-w-ipg">-o-</span> are pronounced:</p>
			<ul class="example-1-ipg reduce-mar-top-ipg">
				<li>long at the end of a syllable: <span class="italic-w-ipg">de-va, lo-ka, do-so;</span></li>
				<li>short when they occur before consonants and the syllable ends with a consonant: <span class="italic-w-ipg">met-tā, phoṭ-ṭab-ba.</span></li>
			</ul>

			<p class="paragraph-2-ipg">The Consonants:</p>

			<p class="paragraph-1-ipg reduce-mar-top-ipg">
				Pāli uses 25 so called grouped consonants that add the vowel "a" to carry sound and are divided into groups according to their form of creation:
			</p>

			<!-- Add consonant here-->
			<div class="responsive-table-ipg">
				<!-- table-2 left-header, right-data-->
				<table class="vowel-list-2 table-regular-ipg">
					<tbody><tr>
						<th class="list-chart-1-ipg">Gutturals</th>
						<td class="list-chart-2-ipg">ka</td>
						<td class="list-chart-2-ipg">kha</td>
						<td class="list-chart-2-ipg">ga</td>
						<td class="list-chart-2-ipg">gha</td>
						<td class="list-chart-2-ipg">ṅa</td>
					</tr>
					<tr>
						<th class="list-chart-1-ipg">Palatals</th>
						<td class="list-chart-2-ipg">ca</td>
						<td class="list-chart-2-ipg">cha</td>
						<td class="list-chart-2-ipg">ja</td>
						<td class="list-chart-2-ipg">jha</td>
						<td class="list-chart-2-ipg">ña</td>
					</tr>
					<tr>
						<th class="list-chart-1-ipg">Retroflex</th>
						<td class="list-chart-2-ipg">ṭa</td>
						<td class="list-chart-2-ipg">ṭha</td>
						<td class="list-chart-2-ipg">ḍa</td>
						<td class="list-chart-2-ipg">ḍha</td>
						<td class="list-chart-2-ipg">ṇa</td>
					</tr>
					<tr>
						<th class="list-chart-1-ipg">Dentals</th>
						<td class="list-chart-2-ipg">ta</td>
						<td class="list-chart-2-ipg">tha</td>
						<td class="list-chart-2-ipg">da</td>
						<td class="list-chart-2-ipg">dha</td>
						<td class="list-chart-2-ipg">na</td>
					</tr>
					<tr>
						<th class="list-chart-1-ipg">Labials</th>
						<td class="list-chart-2-ipg">pa</td>
						<td class="list-chart-2-ipg">pha</td>
						<td class="list-chart-2-ipg">ba</td>
						<td class="list-chart-2-ipg">bha</td>
						<td class="list-chart-2-ipg">ma</td>
					</tr>
				</tbody></table>
			</div>

			<p class="paragraph-1-ipg">
				They get supplemented by: <span class="italic-w-ipg">ya, ra, la, va, sa, ha, ḷa</span> and<span class="italic-w-ipg">aṃ</span>, of which <span class="italic-w-ipg">ra, la, ḷa</span> are liquids,<span class="italic-w-ipg">ya</span> and <span class="italic-w-ipg">va</span> semivowels,<span class="italic-w-ipg">sa</span> is a sibilant, <span class="italic-w-ipg">ha</span> an aspirate and <span class="italic-w-ipg">aṃ</span> is called a <span class="italic-w-ipg">niggahīta</span>. Further ya can be grouped with the palatals, <span class="italic-w-ipg">ra, la, ḷa</span> with the retroflex and <span class="italic-w-ipg">va</span> with the labials.
			</p>

			<p class="paragraph-1-ipg">
				The consonants found in the first and third column are unaspirates, those in the second and fourth are aspirates, those in the last column are called nasals.
			</p>

			<ul class="example-1-ipg">
				<li>All aspirated consonants are pronounced with an audible expulsion of breath following the normal unaspirated sound.</li>
				<li>The guttural consonants: - <span class="italic-w-ipg">ka, kha, ga, gha, ha</span> - are produced from deep within the throat and hardly any movement of the tongue.</li>
				<li>The palatal consonants: - <span class="italic-w-ipg">ca, cha, ja, jha, ya</span> - are pronounced with the front parts of the tongue slightly touching the upper-gum/palate.</li>
				<li>The retroflex or cerebral consonants: - <span class="italic-w-ipg">ṭa, ṭha, ḍa, ḍha, ra, la,ḷa</span> - are pronounced with the tip of the tongue turned back and touching the upper <a href="#section3-note-12" class="notes-ipg" id="section3-note-12-rtn"><span class="italic-w-ipg">palate</span><sup class="sup-spacing-ipg">12</sup></a>.</li>
				<li>The dental consonants: - <span class="italic-w-ipg">ta, tha, da, dha, sa</span> - are pronounced with the tongue touching the upper front teeth.</li>
				<li>The labial consonants: - <span class="italic-w-ipg">pa, pha, ba, bha, ma, va</span> - are formed by movement of both the lips only.</li>
				<li>The nasal consonants: - <span class="italic-w-ipg">ṅa, ña, ṇa, na, ma</span> - are uttered by ways of articulating them in the same way as the preceding consonants of the same group get produced, but with the sound resonating through the <a href="#section3-note-13" class="notes-ipg" id="section3-note-13-rtn"><span class="italic-w-ipg">nose</span><sup class="sup-spacing-ipg">13</sup></a>.</li>
				<li>The niggahīta: - <span class="italic-w-ipg">aṃ</span> - is resonating like ng.</li>
			</ul>

			<p class="paragraph-1-ipg">As above the following similarity to English may serve as pronunciation aid:</p>

			<div class="responsive-table-ipg">
				<!-- table-1 left-data, right-data-->
				<table class="vowel-list-2 table-regular-ipg">
					<tbody><tr>
						<td><span class="italic-w-ipg">ka</span> - as the "k" in king</td>
						<td><span class="italic-w-ipg">ga</span> - as the "g" in get</td>
					</tr>
					<tr>
						<td><span class="italic-w-ipg">ca</span> - as the "ch" in church</td>
						<td><span class="italic-w-ipg">ja</span> - as the "j" in jail</td>
					</tr>
					<tr>
						<td><span class="italic-w-ipg">ta</span> - as the "t" in task</td>
						<td><span class="italic-w-ipg">da</span> - as the "d" in day</td>
					</tr>
					<tr>
						<td><span class="italic-w-ipg">pa</span> - as the "p" in part</td>
						<td><span class="italic-w-ipg">ba</span> - as the "b" in but</td>
					</tr>
					<tr>
						<td><span class="italic-w-ipg">tha</span> - as in "th" Thai</td>
						<td><span class="italic-w-ipg">pha</span> - as "ph" in <a href="#section3-note-14" class="notes-ipg" id="section3-note-14-rtn"><span class="italic-w-ipg">uphill</span><sup class="sup-spacing-ipg">14</sup></a></td>
					</tr>
					<tr>
						<td><span class="italic-w-ipg">ṅa</span> - as "ng" in singer</td>
						<td><span class="italic-w-ipg">ña</span> - as "n" in Spanish señor</td>
					</tr>
					<tr>
						<td><span class="italic-w-ipg">ṇa</span> - as "n" in kind, mind</td>
						<td><span class="italic-w-ipg">na</span> - as "n" in noun</td>
					</tr>
					<tr>
						<td><span class="italic-w-ipg">ṃ</span> - as in hung, ring</td>
						<td><span class="italic-w-ipg">v</span> - is a very soft -v- or <a href="#section3-note-15" class="notes-ipg" id="section3-note-15-rtn"><span class="italic-w-ipg">-w-</span><sup class="sup-spacing-ipg">15</sup></a></td>
					</tr>
				</tbody></table>
			</div>

			<p class="paragraph-1-ipg">Example of the guttural consonants ka and kha in combination with vowels:</p>

			<div class="responsive-table-ipg">
				<!-- table-1 left-data, right-data-->
				<table class="table-regular-ipg">
					<tbody><tr>
						<td class="list-chart-2-ipg">ka</td>
						<td class="list-chart-2-ipg">kā</td>
						<td class="list-chart-2-ipg">ki</td>
						<td class="list-chart-2-ipg">kī</td>
						<td class="list-chart-2-ipg">ku</td>
						<td class="list-chart-2-ipg">kū</td>
						<td class="list-chart-2-ipg">ke</td>
						<td class="list-chart-2-ipg">ko</td>
					</tr>
					<tr>
						<td class="list-chart-2-ipg">kha</td>
						<td class="list-chart-2-ipg">khā</td>
						<td class="list-chart-2-ipg">khi</td>
						<td class="list-chart-2-ipg">khī</td>
						<td class="list-chart-2-ipg">khu</td>
						<td class="list-chart-2-ipg">khū</td>
						<td class="list-chart-2-ipg">khe</td>
						<td class="list-chart-2-ipg">kho</td>
					</tr>
				</tbody></table>
			</div>

			<p class="paragraph-1-ipg">Example of the guttural consonants ka and kha
				in combination with consonants:</p>

			<div class="responsive-table-ipg">
				<!-- table-1 left-data, right-data-->
				<table class="table-regular-ipg">
					<tbody><tr>
						<td class="list-chart-2-ipg">kka</td>
						<td class="list-chart-2-ipg">kkha</td>
						<td class="list-chart-2-ipg">kya</td>
						<td class="list-chart-2-ipg">kri</td>
						<td class="list-chart-2-ipg">kla</td>

					</tr>
					<tr>
						<td class="list-chart-2-ipg">kva</td>
						<td class="list-chart-2-ipg">khya</td>
						<td class="list-chart-2-ipg">khva</td>
						<td class="list-chart-2-ipg">ṅka</td>
						<td class="list-chart-2-ipg">ṅkha</td>
					</tr>
				</tbody></table>
			</div>

			<!-- footnotes section 3 -->
			<ul class="footnotes-container-ipg">
				<h4 class="footnote-heading-ipg">Footnotes</h4>
				<li id="section3-note-9" class="footnotes-ipg"><sup>9</sup> Please refer to footnote 3. <a class="backarrow-ipg" href="#section3-note-9-rtn">↩</a></li>
				<li id="section3-note-10" class="footnotes-ipg"><sup>10</sup> The set of vowels can be further subdivided into the pure vowels (<span class="italic-w-ipg">a, ā</span>) sonant vowels (<span class="italic-w-ipg">i, ī, u, ū</span>) and diphthongs (e, o). This is of interest because the sonants remain vowels if followed by a consonant, but change into the semivowels y and v when followed by a vowel (<span class="italic-w-ipg">vi-anta - vyanta / su-āgato – svāgato</span>). Thus the diphthongs are derived from the union of the first two groups of vowels: <span class="italic-w-ipg">a +i, ā + i : = e; a +u, ā + ū:  =  o</span> <a class="backarrow-ipg" href="#section3-note-10-rtn">↩</a></li>
				<li id="section3-note-11" class="footnotes-ipg"><sup>11</sup> The <span class="italic-w-ipg">"a"</span> may be pronounced slightly differently according to the position amongst the combined syllables in a word, whether in the middle, at the end or following an aspirate or an unaspirated consonant. The pronunciation of letters should be understood as an exercise only to develop a feeling for the correct touch of the organs of the mouth, the correct pronunciation will develop when texts are read and proper awareness is given to this movement. <a class="backarrow-ipg" href="#section3-note-11-rtn">↩</a></li>
				<li id="section3-note-12" class="footnotes-ipg"><sup>12</sup> <span class="italic-w-ipg">la, ḷa</span> often get swapped. When pronouncing <span class="italic-w-ipg">-ḷa-</span> the tongue moves from above the teeth to the lips to perform a trembling sound. <a class="backarrow-ipg" href="#section3-note-12-rtn">↩</a></li>
				<li id="section3-note-13" class="footnotes-ipg"><sup>13</sup>  A general rule is that the nasal consonants can only be combined with consonants of the same group. <a class="backarrow-ipg" href="#section3-note-13-rtn">↩</a></li>
				<li id="section3-note-14" class="footnotes-ipg"><sup>14</sup>  Here the analogy to the English pronunciation does not hold true because "<span class="italic-w-ipg">tha</span>" is never pronounced as in: the, this, etc.; neither is "<span class="italic-w-ipg">pha</span>" pronounced as in phonology, philosophy. Here the unaspirated consonants <span class="italic-w-ipg">ta, da, pa, ba</span> are uttered stressed with effort and directly followed by <span class="italic-w-ipg">-h-</span> sound to pronounce the aspirated consonants. <a class="backarrow-ipg" href="#section3-note-14-rtn">↩</a></li>
				<li id="section3-note-15" class="footnotes-ipg"><sup>15</sup>  The semivowel consonant va is pronounced like "v" as in "vibrate" if preceded by a consonant: – <span class="italic-w-ipg">svākkhāto</span> – well explained - but if preceded by a vowel it sounds like "w" as in "wind": – <span class="italic-w-ipg">sāvaka</span> – disciple. <a class="backarrow-ipg" href="#section3-note-15-rtn">↩</a></li>
			</ul>
		</section>

<style>

</style>