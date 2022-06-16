# Bus-Ticket-Reservation
<!DOCTYPE html>
<html>

<head>
    <title> Ticketing System</title>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" type="text/css" href="css/style.css" />
    <script src="js/add-row.js"></script>
    <script src="js/enable-button.js"></script>
</head>

<body>
    <div class="header">
        <h1>Ticket Reservation</h1>
    </div>
    <form action="process.php" class="register" method="POST">
        <fieldset class="row1">
            <legend>Travel Information</legend>
            <p>
                <label>Bus-name *
                </label>
                <input name="bus" type="text" required="required" />
                <label>Date
                </label>
                <select class="date" name="day">
                    <option value="1">01
                    </option>
                    <option value="2">02
                    </option>
                    <option value="3">03
                    </option>
                    <option value="4">04
                    </option>
                    <option value="5">05
                    </option>
                    <option value="6">06
                    </option>
                    <option value="7">07
                    </option>
                    <option value="8">08
                    </option>
                    <option value="9">09
                    </option>
                    <option value="10">10
                    </option>
                    <option value="11">11
                    </option>
                    <option value="12">12
                    </option>
                    <option value="13">13
                    </option>
                    <option value="14">14
                    </option>
                    <option value="15">15
                    </option>
                    <option value="16">16
                    </option>
                    <option value="17">17
                    </option>
                    <option value="18">18
                    </option>
                    <option value="19">19
                    </option>
                    <option value="20">20
                    </option>
                    <option value="21">21
                    </option>
                    <option value="22">22
                    </option>
                    <option value="23">23
                    </option>
                    <option value="24">24
                    </option>
                    <option value="25">25
                    </option>
                    <option value="26">26
                    </option>
                    <option value="27">27
                    </option>
                    <option value="28">28
                    </option>
                    <option value="29">29
                    </option>
                    <option value="30">30
                    </option>
                    <option value="31">31
                    </option>
                </select>
                <select name="month">
                    <option value="1">January
                    </option>
                    <option value="2">February
                    </option>
                    <option value="3">March
                    </option>
                    <option value="4">April
                    </option>
                    <option value="5">May
                    </option>
                    <option value="6">June
                    </option>
                    <option value="7">July
                    </option>
                    <option value="8">August
                    </option>
                    <option value="9">September
                    </option>
                    <option value="10">October
                    </option>
                    <option value="11">November
                    </option>
                    <option value="12">December
                    </option>
                </select>
                <label>Bus-type *
                </label>
                <select name="type">
                    <option value="Sleeper">Sleeper
                    </option>
                    <option value="Semi Sleeper">Semi Sleeper
                    </option>
                </select>

            </p>
            <p>
                <label>From*
                </label>
                <input name="from" required="required" type="text" />
                <label>To *
                </label>
                <input name="to" required="required" type="text" />
                <label>Via *
                </label>
                <select name="root">
                    <option value="Place 1">Place 1
                    </option>
                    <option value="Place 2">Place 2
                    </option>
                    <option value="Place 3">Place 3
                    </option>
                </select>
            </p>
            <p>
                <label>Mobile *
                </label>
                <input name="mob" required="required" type="text" />
                <label>Confirm*
                </label>
                <input name="mob" required="required" type="text" />
            </p>
            <div class="clear"></div>
        </fieldset>
        <fieldset class="row2">
            <legend>Fare Details</legend>
            <p>
                <input type="button" value="Add Fare" onClick="addRow('dataTable')" />
                <input type="button" value="Remove Fare" onClick="deleteRow('dataTable')" />
            </p>
            <table id="dataTable" class="form" border="1">
                <tbody>
                    <tr>
                        <p>
                            <td><input type="checkbox" required="required" name="chk[]" checked="checked" /></td>
                            <td>
                                <label>Name</label>
                                <input type="text" required="required" name="BX_NAME[]">
                            </td>
                            <td>
                                <label for="BX_age">Age</label>
                                <input type="text" required="required" class="small" name="BX_age[]">
                            </td>
                            <td>
                                <label for="BX_gender">Gender</label>
                                <select id="BX_gender" name="BX_gender[]" required="required">
                                    <option value="Male">Male</option>
                                    <option value="Female">Female</option>
                                </select>
                            </td>
                            <td>
                                <label for="BX_birth">Berth Pre</label>
                                <select id="BX_birth" name="BX_birth[]" required="required">
                                    <option>Window</option>
                                    <option>No Choice</option>
                                </select>
                            </td>
                        </p>
                    </tr>
                </tbody>
            </table>
            <div class="clear"></div>
        </fieldset>
        <fieldset class="row4">
            <legend>Terms and Conditions</legend>
            <p class="agreement">
                <input type="checkbox" onclick="enableButton()" value="" />
                <label>* I accept the <a href="#">Terms and Conditions</a></label>
            </p>

            <div class="clear"></div>
        </fieldset>
        <div class="row">
            <input class="submit" id="button" type="submit" value="Confirm/Pay &raquo;" disabled>
        </div>
        <div class="clear"></div>
    </form>
    <div class="image">
        <img class="bus1" src="images/bus-truning.gif" alt="parked bus">
    </div>
    <div class="footer">
        <p>The identification details are required during journey. One of the passenger booked on the ticket should
            have any of the identity cards ( Passport / PAN Card / Driving License / Photo ID card issued by Central
            / State Govt / Student Identity Card with photograph) during the journey in original </p>
        <p>© 2020 Passenger Tim, all rights reserved</p>
    </div>
</body>

</html>