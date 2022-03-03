- 👋 Hi, I’m @Joeighisranodm
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Joeighisranodm/Joeighisranodm is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
(IBAction)openSupport:(id)sender {
    NSString* subject = [@"Autoclick Support and Feedback" stringByAddingPercentEncodingWithAllowedCharacters:[NSCharacterSet URLQueryAllowedCharacterSet]];

    NSURL* url = [NSURL URLWithString:[NSString stringWithFormat:@"mailto:autoclick@mahdi.jp?subject=%@", subject]];

    [[NSWorkspace sharedWorkspace] openURL:url];
}

- (IBAction)openGitHub:(id)sender {
    NSURL *url = [NSURL URLWithString:@"https://github.com/inket/Autoclick"];
    [[NSWorkspace sharedWorkspace] openURL:url];
}

- (IBAction)openBuyMeACoffee:(id)sender {
    NSURL *url = [NSURL URLWithString:@"https://www.buymeacoffee.com/mahdibchatnia"];
    [[NSWorkspace sharedWorkspace] openURL:url];
}

#pragma mark - Icon Handling

- (void)defaultIcon {

