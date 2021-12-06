[![Header](https://github.com/jakemclelland/jakemclelland/blob/main/assets/latest_story.png "Header")](https://jakemclelland.github.io/cv/)

### Hi there 👋

I'm Jake. . . a programmer

<p>It wasn't long ago that a great way to send data to someone was to attach a small note to the leg to a carrier pigeon. Fortunately, these days, we don’t need to employ millions of pigeons in order to sync tables between two database systems. Now all those pigeons are free to retire to their big city havens to snag tasty morsels from unsuspecting pedestrians.</p>

```c#
public class Jake
{
	public Jake()
	{
		Code = new List<string>{"i dream in C#", "and SQL", "and SSIS", "my nightmares usually involve JavaScript", "but Swift seems pretty cool"};
		Favorites = new List<string>{"the ancient art of bonsai"};
		Contacts = new List<string>{"https://www.linkedin.com/in/jakemclelland/"};
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
				aboutMe.AppendLine("And what's cool right now?");
				Favorites.ForEach(_ => aboutMe.AppendLine($"  {_}"));
				break;
			case InquiryType.Contact:
				aboutMe.AppendLine("How may I contact you?");
				Contacts.ForEach(_ => aboutMe.AppendLine($"  find me on {_}"));
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
```
<a href="https://dotnetfiddle.net/HGqeVp">run on dotnetfiddle.net</a>

<a href="https://stackoverflow.com/users/2859272/jakemc"><img src="https://stackoverflow.com/users/flair/2859272.png?theme=dark" width="208" height="58" alt="profile for JakeMc at Stack Overflow, Q&amp;A for professional and enthusiast programmers" title="profile for JakeMc at Stack Overflow, Q&amp;A for professional and enthusiast programmers"></a>

<div class="badge-base LI-profile-badge" data-locale="en_US" data-size="large" data-theme="dark" data-type="VERTICAL" data-vanity="jakemclelland" data-version="v1"><a class="badge-base__link LI-simple-link" href="https://www.linkedin.com/in/jakemclelland?trk=profile-badge">Jake McLelland</a></div>
              
<!--
**jakemclelland/jakemclelland** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
