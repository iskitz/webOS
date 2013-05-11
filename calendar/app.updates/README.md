webOS Calendar App Bug Fixes
============================
Bug fixes for the core, un-patched webOS 3.0.5 Calendar application.


+ 2013.05.11: [__3.0.5-2013.05.11__](https://raw.github.com/iskitz/webOS/master/calendar/app.updates/calendar.3.0.11007.2013.05.11.iskitz.bug.fixes.patch)
   + __Improved:__ Creating an event via a _Just Type Quick Action_ now closes any existing event detail popup.
   + __Improved:__ Tapping the calendar icon when the calendar is in card view
      + Brings it into focus, switches to Day view and updates the date shown as follows
         + If you were in Month view, Day view shows the first day of that month or the day of the month you were last viewing.
         + If you were in Week  view, Day view shows the first day of that week or the day of the week you were last viewing.
         + If you were in Day   view, Day view shows the same day that was being viewed.
      + __tip:__ To view "today" in any view, double-tap that view's icon in the view switcher bar at the bottom of the calendar.
   + __Improved: Stability__
      + When the calendar is closed, tapping on event alarms, search results and quick actions always opens the calendar and shows the tapped event.
      + Switching views immediately shows the intended date instead of first quickly showing the old date.
      + Week & Month views now safely check whether available events occur on the currently displayed day(s).
      + All intra-app asynchronous notifications are delivered until explicitly ignored.
         + No longer only sending the first notification.
   + __Improved: Other things__
      + Began minor refactoring needed to re-enable loading calendar within a browser.
         + Primarily doing this for better calendar debugging via desktop browsers.
         + Currently loads all resources but shows a blank view when viewed in the webOS browser; more work to be done.
