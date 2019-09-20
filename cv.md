# Sergey Antonov

## Contact Info

1. tel: 89879108892
2. tel: 89376525911
3. E-mail: antonov-ser-v@yandex.ru
4. E-mail: antnov.sergei@gmail.com

## Summary

### My goal

My goal it to become Front-End Developer. I want to learn in web layout. At the moment, popular and prestigious

position. Pros this specialization in is that all time works the brain. Since 2010 I have been constantly 

studying different programming platforms. Qualities that I possess: commitment, focus on results.

## Skills

Programming languages:

C#, PHP, Excel VBA 

### Data base

Posgress SQL,Oracle # Code examples #

### My latest Code C#

```scharp
private void button1_Click(object sender, EventArgs e)
{
    string[] fold = Directory.GetDirectories(textBox1.Text);
    foreach (string path_folder in fold)
    {
        string dddd = path_folder;
        string[] _fail = Directory.GetFiles(path_folder,"*.*",SearchOption.AllDirectories);
        if(_fail.Length != 0) {
                try
                {
                    foreach (string _move in _fail)
                    {
                        if (Path.GetFileName(_move) != "Thumbs.db")
                        {
                            File.Move(_move, textBox2.Text + @"\" + Path.GetFileName(_move));
                        }
                        else
                        {
                            File.Delete(_move);
                        }
                    }
                }
                catch (Exception)
                {
                    MessageBox.Show("Ошибка");  
                }
            }
            else
            {
                if (checkBox1.Checked) {
                    Directory.Delete(path_folder);
                }
            }
        }
        MessageBox.Show("Готово");
    }
    //Откуда извлеч
    private void button2_Click(object sender, EventArgs e)
    {
        FolderBrowserDialog whence = new FolderBrowserDialog();
        whence.ShowNewFolderButton = false;
        if (whence.ShowDialog() == DialogResult.OK)
        {
            textBox1.Text = whence.SelectedPath;
        }
        else{
            MessagrBox("Ошибка пути");
        }
    }

    private void button3_Click(object sender, EventArgs e)
    {
        FolderBrowserDialog where = new FolderBrowserDialog();
        where.ShowNewFolderButton = false;
        if (where.ShowDialog() == DialogResult.OK)
        {
            textBox2.Text = where.SelectedPath;
        }
        else
        {
        }
    }
}
```
