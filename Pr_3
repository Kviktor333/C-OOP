using System;

namespace ConsoleApp2
{
    class Book
    {
        private string title;
        private Author author;
        private Content content;

        public Book(string title, string author, string content)
        {
            this.title = title;
            this.author = new Author(author);
            this.content = new Content(content);
        }
        public string Title => title;
        public string AuthorName
        {
            get => author.Name;
            set => author.Name = value;
        }
        public string ContentText
        {
            get => content.Text;
            set => content.Text = value;
        }
        public void Show()
        {
            Console.ForegroundColor = ConsoleColor.Red;
            Console.WriteLine($"Title: {title}");
            Console.ForegroundColor = ConsoleColor.Yellow;
            Console.WriteLine($"Author: {author.Name}");
            Console.ForegroundColor = ConsoleColor.Green;
            Console.WriteLine($"Content: {content.Text}");
            Console.ResetColor();
        }
    }
    class Author
    {
        public string Name { get; set; }
        public Author(string name)
        {
            Name = name;
        }
    }

    class Content
    {
        public string Text { get; set; }
        public Content(string text)
        {
            Text = text;
        }
    }
    class Program
    {
        static void Main()
        {
            Book book = new Book("Intermezzo", "Mykhailo Kotsiubynsky", "An impressionistic novel by the Ukrainian writer, written in 1908 in Chernihiv");
            book.Show();
        }
    }
}
