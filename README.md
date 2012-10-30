# Bootstrap Datepicker v1.0 #

A jQuery UI Datepicker widget with Twitter Bootstrap theme.  It's based on jQuery UI 1.9.1 and Twitter Bootstrap 2.1.1.

See demo page for more examples.

## Usage ##

    <input type="text" name="date" class="datepicker" />

    <script>
        $(document).ready(function() {
            $(".datepicker").datepicker();
        });
    </script>

Using fancy bootstrap input/button combo:

    <div class="control-group">
        <label class="control-label" for="datepicker">Date</label>
        <div class="controls">
            <div class="input-append">
                <input id="datepicker" class="input-small" type="text">
                <button id="datepickerbtn" class="btn" type="button"><i class="icon-calendar"></i></button>
            </div>
        </div>
    </div>

    <script>
        $(document).ready(function() {
            $("#datepicker").datepicker();
            $("#datepickerbtn").click(function(event) {
                event.preventDefault();
                $("#datepicker").focus();
            })
        });
    </script>
