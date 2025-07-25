[![Header](https://github.com/jakemclelland/jakemclelland/blob/main/assets/Pigeon%2020220904-02.png "Header")](https://jakemclelland.github.io/cv/)

### Hi there 👋

I'm Jake. . . a programmer

<p>It wasn't long ago that a great way to send data to someone was to attach a small note to the leg to a carrier pigeon. Fortunately, these days, we don’t need to employ millions of pigeons in order to sync data between two systems. Now all those pigeons are free to retire to their big city havens to snag tasty morsels from unsuspecting pedestrians.</p>

<p>Also a certified <a href="https://www.credly.com/badges/305cd2d9-929d-4b65-9bed-f06c3611b91f/public_url">Professional Scrum Master PCM (PSM I)</a></p>

<p>Check out my resume page <a href="https://jakemclelland.github.io/resume/">here</a>.</p>

# Blog posts
<!-- BLOG-POST-LIST:START -->
- [Sometimes the Best Work Ends with No Work at All](https://dev.to/jakemclelland/sometimes-the-best-work-ends-with-no-work-at-all-2hig)
- [Some thoughts on AI](https://dev.to/jakemclelland/some-thoughts-on-ai-5g6i)
- [Syntactic Elegance-The Developer’s Dream](https://dev.to/jakemclelland/syntactic-elegance-the-developers-dream-329b)
- [Handling Duplicate Records](https://dev.to/jakemclelland/handling-duplicate-records-4l57)
- [Combining two datasets into one](https://dev.to/jakemclelland/combining-two-datasets-into-one-3826)
<!-- BLOG-POST-LIST:END -->

# StackOverflow Activity
<!-- STACKOVERFLOW:START -->
- [Answer by JakeMc for Skip current line in debugger](https://stackoverflow.com/questions/31474563/skip-current-line-in-debugger/79709687#79709687)
- [Answer by JakeMc for Is there a way to debug code in VsCode initiated with Vite?](https://stackoverflow.com/questions/66147328/is-there-a-way-to-debug-code-in-vscode-initiated-with-vite/79468088#79468088)
- [Answer by JakeMc for Deploy .Net Aspire project to an Azure VM](https://stackoverflow.com/questions/78810200/deploy-net-aspire-project-to-an-azure-vm/78816965#78816965)
- [Answer by JakeMc for Why can&#39;t I use table names of aliased tables in WHERE clause?](https://stackoverflow.com/questions/78678900/why-cant-i-use-table-names-of-aliased-tables-in-where-clause/78679140#78679140)
- [Answer by JakeMc for How to alternate div display based on class name](https://stackoverflow.com/questions/77867345/how-to-alternate-div-display-based-on-class-name/77867544#77867544)
<!-- STACKOVERFLOW:END -->

# If I Were a Program
<a href="https://dotnetfiddle.net/HGqeVp">run on dotnetfiddle.net :point_down:</a>
```c#

public class Program
{
	public class Jake
	{
		public Jake()
		{
			Code = new List<string>{"i dream in C#", "and SQL", "and SSIS", "my nightmares usually involve JavaScript", "but Swift and React Native seems pretty interesting"};
			Favorites = new List<string>{"reading and collecting super old books", "i'm a huge fan of the ancient art of bonsai", "i also have an aquascape aquarium"};
			Contacts = new List<string>{"find me on https://www.linkedin.com/in/jakemclelland", "or hire me at https://www.codepoetllc.com"};
		}

		public List<string> Code { get; set; }
		public List<string> Favorites { get; set; }
		public List<string> Contacts { get; set; }

		public string TellMeAboutYourself(InquiryType inquiry)
		{
			StringBuilder aboutMe = new StringBuilder();
			switch (inquiry)
			{
				case InquiryType.Code:
					aboutMe.AppendLine("So tell me, what are you doing these days?");
					Code.ForEach(_ => aboutMe.AppendLine($"  {_}"));
					break;
				case InquiryType.Favorites:
					aboutMe.AppendLine("And what have you been up to lately?");
					Favorites.ForEach(_ => aboutMe.AppendLine($"  {_}"));
					break;
				case InquiryType.Contact:
					aboutMe.AppendLine("How may I contact you?");
					Contacts.ForEach(_ => aboutMe.AppendLine($"  {_}"));
					break;
			}
			
			return aboutMe.ToString();
		}
	}

	public static void Main()
	{
		var me = new Jake();
		Console.WriteLine(me.TellMeAboutYourself(InquiryType.Code));
		Console.WriteLine(me.TellMeAboutYourself(InquiryType.Favorites));
		Console.WriteLine(me.TellMeAboutYourself(InquiryType.Contact));
	}

	public enum InquiryType
	{
		Code,
		Favorites,
		Contact
	}	
}
```
<a href="https://dotnetfiddle.net/HGqeVp">run on dotnetfiddle.net :point_up_2:</a>

<p><a href="https://forms.gle/XbNLBM1YMcb7UNzz7">Hire Me</a></p>

<p>Find me on:</p>
<a href="https://stackoverflow.com/users/2859272/jakemc"><img src="https://stackoverflow.com/users/flair/2859272.png?theme=dark" width="208" height="58" alt="profile for JakeMc at Stack Overflow, Q&amp;A for professional and enthusiast programmers" title="profile for JakeMc at Stack Overflow, Q&amp;A for professional and enthusiast programmers"></a>

<div class="badge-base LI-profile-badge" data-locale="en_US" data-size="large" data-theme="dark" data-type="VERTICAL" data-vanity="jakemclelland" data-version="v1"><a class="badge-base__link LI-simple-link" href="https://www.linkedin.com/in/jakemclelland?trk=profile-badge"><img alt="Linked In Logo" src="https://github.com/jakemclelland/jakemclelland/blob/main/assets/linked-in-logo.jpg"></a></div>

<div>
   <a href="https://www.codepoetllc.com"><img alt="Codepoet Logo" src="https://github.com/jakemclelland/jakemclelland/blob/main/assets/codepoet-logo.jpg"></a>
</div>

---
      
<div>
	<i>Thanks to <a href="https://dev.to/dawsoncodes">@dawsoncodes</a> for the ideas, and <a href="https://github.com/gautamkrishnar">Gautam Krishna</a> for the blog-post-workflow</i>
</div>
