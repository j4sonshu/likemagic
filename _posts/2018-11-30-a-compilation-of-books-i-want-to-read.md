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
      <td><p onclick="searchGoogle('11/22/63: A Novel Stephen King')">11/22/63: A Novel</p></td>
      <td>Stephen King</td>
      <td>Science Fiction</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('The Dice Man Luke Rhinehart')">The Dice Man</p></td>
      <td>Luke Rhinehart</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('The Mist Stephen King')">The Mist</p></td>
      <td>Stephen King</td>
      <td>Horror</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('The Colour Out of Space H. P. Lovecraft')">The Colour Out of Space</p></td>
      <td>H. P. Lovecraft</td>
      <td>Science Fiction</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('Earth Abides: A Novel George R. Stewart')">Earth Abides: A Novel</p></td>
      <td>George R. Stewart</td>
      <td>Science Fiction</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('Endure: Mind, Body, and the Curiously Elastic Limits of Human Performance Alex Hutchinson')">Endure: Mind, Body, and the Curiously Elastic Limits of Human Performance</p></td>
      <td>Alex Hutchinson</td>
      <td>Sports</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('A Life Without Limits: A World Champion's Journey Chrissie Wellington')">A Life Without Limits: A World Champion's Journey</p></td>
      <td>Chrissie Wellington</td>
      <td>Sports</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('Swim, Bike, Run, Eat: The Complete Guide to Fueling Your Triathlon Tom Holland')">Swim, Bike, Run, Eat: The Complete Guide to Fueling Your Triathlon</p></td>
      <td>Tom Holland</td>
      <td>Sports</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('How Bad Do You Want It?: Mastering the Psychology of Mind over Muscle Matt Fitzgerald')">How Bad Do You Want It?: Mastering the Psychology of Mind over Muscle</p></td>
      <td>Matt Fitzgerald</td>
      <td>Sports</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('The Quiet Earth Craig Harrison')">The Quiet Earth</p></td>
      <td>Craig Harrison</td>
      <td>Science Fiction</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('East of Eden John Steinbeck')">East of Eden</p></td>
      <td>John Steinbeck</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('Brave New World Aldous Huxley')">Brave New World</p></td>
      <td>Aldous Huxley</td>
      <td>Science Fiction</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('Never Let Me Go Kazuo Ishiguro')">Never Let Me Go</p></td>
      <td>Kazuo Ishiguro</td>
      <td>Science Fiction</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('The Kite Runner Khaled Hosseini')">The Kite Runner</p></td>
      <td>Khaled Hosseini</td>
      <td>Historical Fiction</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('And the Mountains Echoed Khaled Hosseini')">And the Mountains Echoed</p></td>
      <td>Khaled Hosseini</td>
      <td>Historical Fiction</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('The Ocean at the End of the Lane Neil Gaiman')">The Ocean at the End of the Lane</p></td>
      <td>Neil Gaiman</td>
      <td>Fantasy</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('The Elephant Vanishes Haruki Murakami')">The Elephant Vanishes</p></td>
      <td>Haruki Murakami</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('The First Fifteen Lives of Harry August Claire North')">The First Fifteen Lives of Harry August</p></td>
      <td>Claire North</td>
      <td>Science Fiction</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('The Master Key System Charles F. Haanel')">The Master Key System</p></td>
      <td>Charles F. Haanel</td>
      <td>Non-Fiction</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('The Autobiography of Malcolm X Malcolm X')">The Autobiography of Malcolm X</p></td>
      <td>Malcolm X</td>
      <td>Autobiography</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('Flowers for Algernon Daniel Keyes')">Flowers for Algernon</p></td>
      <td>Daniel Keyes</td>
      <td>Science Fiction</td>
    </tr>
    <tr>
      <td><p onclick="searchGoogle('Enquire Within Upon Everything Daniel Keyes')">Enquire Within Upon Everything</p></td>
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
