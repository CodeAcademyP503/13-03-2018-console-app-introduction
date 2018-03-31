1. Birinci sual
2. Ikinci Sual

```
public void SaveData(object obj,EventArgs e)
        {
            var btn = obj as Button; 
            var name = NameBox.Text;
            var surname = SurnameBox.Text;
            var age = Convert.ToInt32(AgeBox.Text);
            
            var newUser=new User(name, surname, age);
            newUser.Id = Count;
            NameBox.Text = "";
            SurnameBox.Text = "";
            AgeBox.Text = "";
            Count++;
            SelectForDelete.Items.Add(newUser.Id);

        }
```
