# CSS Tips

1. Form elements overlapping:
  
    Form element are inline. So if you use `<br/>` to change line the elements will overlap. You can see that on adding margin     it doesn't work. 
    Better approach:
    ```css
    form {
      display: flex;
      flex-direction: column;
    }
    ```
