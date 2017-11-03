# CSS and HTML

## Numbered list with theoretically infinite number of sublists and respective enumeration.

### CSS:

      ol { counter-reset: item; list-style-type: upper-roman; }
      li { counter-increment: item; }
      ol ol { list-style: none; }
      ol ol > li:before { content: counters(item, ".") ". "; margin-left: -20px;  }
      
### HTML:

      <ol>
        <li>First list
          <ol>
            <li>Second list, p.1</li>
            <li>Second list, p.2</li>
          </ol>
        </li>
      </ol>
      
