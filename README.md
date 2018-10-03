# slack-themes
slack drak mode theme

slack-grey
Dark grey theme for the Slack GNU/Linux desktop client

About
This theme answers the need for decent night mode theme in the Slack client. If you're tired of being blinded by glaring white backgrounds and start black text, then this theme is for you. The theme is basedon laCour's drak theme with some modifications for reduced text contrast. This theme has been tested and working with Slack 3.3.1 on Debian GNU/Linux 9.

Licence
This theme is Unlicensed. Under no conditions are warranties implied or expressed for when Slack eventually breaks it with the next update. See LICENSE

Installation
You may need sudo privileges for this.

Append the following to ssb-interop.js, which is found in the /usr/lib/slack/resources/app.asar.unpacked/src/static/ directory:
document.addEventListener('DOMContentLoaded', function() {
 $.ajax({
   url: '',
   success: function(css) {
     $("<style></style>").appendTo('head').html(css);
   }
 });
});
Launch the Slack client to bask in dark mode glory.
