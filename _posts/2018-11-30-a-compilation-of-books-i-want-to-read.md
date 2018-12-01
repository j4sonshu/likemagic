---
layout: post
title: "A Compilation of Books I Want to Read"
comments: true
author: "Jason Shu"
tags: [books]
---

Over the course of the past several years, every time someone recommended me a book to read, I found the book on Amazon and bookmarked it, thinking that I'll get to it at some time. Now, I have an extremely large folder of bookmarks of books I never actually got to read.

I've decided to put these books in a table (in this post) so that (1) I have a centralized place where I can see the books, and (2) so that anyone reading this can find the books too. You can sort the table by Title, Author, and Genre.

<table class="the-list">
  <thead>
    <tr>
      <th colspan="3" style= "text-align: center"><h3>My Book List</h3></th>
    </tr>
    <tr>
      <th onclick="sortTable(0)"><i class="sortable">Title</i><i class="sort-by"></i></th>
      <th onclick="sortTable(1)"><i class="sortable">Author</i><i class="sort-by"></i></th>
      <th onclick="sortTable(2)"><i class="sortable">Genre</i><i class="sort-by"></i></th>
    </tr>
  </thead>

  <tbody id="myTableBody">
    <tr>
      <td><a href="https://www.amazon.com/11-22-63-Stephen-King/dp/1501120603">11/22/63: A Novel</a></td>
      <td>Stephen King</td>
      <td>Science Fiction</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Dice-Man-Luke-Rhinehart/dp/0879518642">The Dice Man</a></td>
      <td>Luke Rhinehart</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Mist-Stephen-King/dp/1982103523">The Mist</a></td>
      <td>Stephen King</td>
      <td>Horror</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Colour-Out-Space-H-Lovecraft/dp/1447418336">The Colour Out of Space</a></td>
      <td>H. P. Lovecraft</td>
      <td>Science Fiction</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Earth-Abides-George-R-Stewart/dp/0345487133">Earth Abides: A Novel</a></td>
      <td>George R. Stewart</td>
      <td>Science Fiction</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Endure-Curiously-Elastic-Limits-Performance/dp/0062499866">Endure: Mind, Body, and the Curiously Elastic Limits of Human Performance</a></td>
      <td>Alex Hutchinson</td>
      <td>Sports</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Life-Without-Limits-Champions-Journey/dp/1455505587">A Life Without Limits: A World Champion's Journey</a></td>
      <td>Chrissie Wellington</td>
      <td>Sports</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Swim-Bike-Run-Eat-Triathlon/dp/159233606X">Swim, Bike, Run, Eat: The Complete Guide to Fueling Your Triathlon</a></td>
      <td>Tom Holland</td>
      <td>Sports</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/How-Bad-You-Want-Psychology/dp/1937715418">How Bad Do You Want It?: Mastering the Psychology of Mind over Muscle</a></td>
      <td>Matt Fitzgerald</td>
      <td>Sports</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Quiet-Earth-Text-Classics/dp/1922147052">The Quiet Earth</a></td>
      <td>Craig Harrison</td>
      <td>Science Fiction</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/East-Eden-John-Steinbeck/dp/B0093LE9A4">East of Eden</a></td>
      <td>John Steinbeck</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Brave-New-World-Aldous-Huxley/dp/0060850523">Brave New World</a></td>
      <td>Aldous Huxley</td>
      <td>Science Fiction</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Never-Let-Me-Kazuo-Ishiguro/dp/1400078776">Never Let Me Go</a></td>
      <td>Kazuo Ishiguro</td>
      <td>Science Fiction</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Kite-Runner-Khaled-Hosseini/dp/159463193X">The Kite Runner</a></td>
      <td>Khaled Hosseini</td>
      <td>Historical Fiction</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Mountains-Echoed-Khaled-Hosseini/dp/1594632383">And the Mountains Echoed</a></td>
      <td>Khaled Hosseini</td>
      <td>Historical Fiction</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Ocean-End-Lane-Novel/dp/0062459368">The Ocean at the End of the Lane</a></td>
      <td>Neil Gaiman</td>
      <td>Fantasy</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Elephant-Vanishes-Stories-Haruki-Murakami/dp/0679750533">The Elephant Vanishes</a></td>
      <td>Haruki Murakami</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/First-Fifteen-Lives-Harry-August/dp/0316399620">The First Fifteen Lives of Harry August</a></td>
      <td>Claire North</td>
      <td>Science Fiction</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Master-Key-System-Charles-Haanel/dp/1604502754">The Master Key System</a></td>
      <td>Charles F. Haanel</td>
      <td>Non-Fiction</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Autobiography-Malcolm-Told-Alex-Haley/dp/0345350685">The Autobiography of Malcolm X</a></td>
      <td>Malcolm X</td>
      <td>Autobiography</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Flowers-Algernon-Daniel-Keyes/dp/015603008X">Flowers for Algernon</a></td>
      <td>Daniel Keyes</td>
      <td>Science Fiction</td>
    </tr>
    <tr>
      <td><a href ="https://www.amazon.com/Enquire-Within-upon-Everything-1890/dp/187359030X">Enquire Within Upon Everything</a></td>
      <td>Daniel Keyes</td>
      <td>Science Fiction</td>
    </tr>

  </tbody>
</table>

[&uarr; Back to Top](#)

<script>
  function sortTable(n) {
    var table, rows, switching, i, x, y, shouldSwitch, dir, switchcount = 0;
    table = document.getElementById("myTableBody");
    switching = true;
    dir = "asc";
    while (switching) {
      switching = false;
      rows = table.rows;
      for (i = 0; i < (rows.length - 1); i++) {
        shouldSwitch = false;
        x = rows[i].getElementsByTagName("td")[n];
        y = rows[i + 1].getElementsByTagName("td")[n];
        if (dir == "asc") {
          if (x.innerHTML.toLowerCase() > y.innerHTML.toLowerCase()) {
            shouldSwitch = true;
            break;
          }
        } else if (dir == "desc") {
            if (x.innerHTML.toLowerCase() < y.innerHTML.toLowerCase()) {
            shouldSwitch = true;
            break;
          }
        }
      }
      if (shouldSwitch) {
        rows[i].parentNode.insertBefore(rows[i + 1], rows[i]);
        switching = true;
        switchcount++;
      } else {
        if (switchcount == 0 && dir == "asc") {
          dir = "desc";
          switching = true;
        }
      }
    }
  }
  window.onload = sortTable(0);

  function searchGoogle(str) {
    window.open("http://google.com/search?q=" + str,"_blank");

  }
</script>
