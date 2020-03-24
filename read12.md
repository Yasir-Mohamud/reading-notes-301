# EJS PARTIALS
_________________

- Comes in handy when you want reuse the same html across multiple pages.
- The `  <%- %> ` tags allows outputting unescaped content into the page .
- You can put them in an `include(the-ejs-file).
-  Its going to look like this -
``` html
<!-- views/partials/footer.ejs -->
 <footer class="footer">
        <p>© 90210 Lawyer Stuff.</p>
    </footer>
```

``` html
<!-- views/post.ejs --> 

          </div>
            <%- include('partials/footer') %>
        </div>
    </body>
    </html>
```
