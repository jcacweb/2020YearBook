# Instruction on how to replicate this e-book format.

1. Make a copy of the this repository.
2. Output the hall book as list of individual images with name as `CompiledFinal#.png` where `#` is the page number. So first page will be `CompiledFinal1.png`. MacOS highlight and rename features should be useful. Place these photos in the pages folder. Besides make sure that 2nd and 3rd page is empty page blank space.
3. Modify `index.html`:

If the maximum number of pages is 102 check `2019Yearbook` repo.
##### 1
```HTML
<!-- Line 24 -->
<div class="hard p103"></div>
<div class="hard p104"></div>
```
Maximum number of pages + 1 and
maximum number of pages + 2 
##### 2
```HTML
<!-- Line 36 -->
<div class="divA">
	<a class="centerA" href="https://firebasestorage.googleapis.com/v0/b/publicity-website.appspot.com/o/yearbook%2FHall%20Book%202020.pdf?alt=media&token=c3a127d3-4cec-4cb5-be56-afe5636f4581"  download="Hall_Year_Book_2019.pdf"   target="_blank">Download</a>
</div>
```
The download url
##### 3
```HTML
<!-- Line 59: to number of pages + 3 -->
	step = 105,
```
This is maximum number of pages + 3
##### 4

```HTML
<!-- Line 168: to number of pages -->
	pages: 102,
```
This is maximum number of pages + 3

4. Modify `docs.css`:
``` CSS
/* Line 99: to maximum number of pages + 1 and maximum number of pages + 2 */
.sample-docs .p103{
	background-position:-960px 0;
}

.sample-docs .p104{
	background-position:-1490px 0;
}
```
5. Modify `covers.jpg`:

Replace the actual covers image into the `covers.jpg`.


If you have trouble feel free to email lowzhao@gmail.com
