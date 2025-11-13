# jquery_dateControl_handler
Extends the .val() function of the native date control

The native HTML date control accepts and outputs dates in the format yyyy-mm-dd. Some databases (SQL Server, for instance) only accept the date as mm/dd/yyyy. This function replaces the .val() function of the native date control (as referenced by jQuery) and makes those conversions on the control level, along with providing a few additional functions as detailed here.

*USAGE

    $("#myNativeDateControl").val("11/13/2025") >> inputs to "2025-11-13"

    const testDate = $("#myNativeDateControl").val() >> outputs "2025-11-13" to "11/13/2025"

*OTHER FUNCTIONS

    $("#myNativeDateControl").val("today")     >> inputs todays date as yyyy-mm-dd 

    "today": sets to the current date.
    "now": same as today.
    "first": first day of the current month.
    "prevfirst": first day of the previous month.
    "prevlast": last day of the previous month.
    "tomorrow": next day.
    "yesterday": previous day.
    "": clears the date.
    Strings like "+3d" or "-1m" or "+2y": adjusts the date by that amount of days, months, or years.
    
