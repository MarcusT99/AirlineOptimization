<h1>Optimizing Flight Selection & Airline Performance</h1>

<h2>Authors</h2>
<ul>
    <li>David Allen</li>
    <li>Jacob Waymire</li>
    <li>Marcus Boswell</li>
    <li>Pravin Dikshit</li>
</ul>

<h2>Project Description</h2>
<p>Commercial aviation has become the most common method of long-distance travel. Frequent flyers often develop perceptions about individual airlines, airports, and even certain times of the year based on their travel experiences. This project aims to explore the rationality behind these perceptions by analyzing airline performance indicators relevant to passengers. We also develop an optimization model that identifies the best flights based on "hidden costs" associated with flying.</p>

<h2>General Repository Information</h2>
<p>This repository includes the following components:</p>
<ul class="folder-list">
    <li><strong>Code Folder:</strong> Contains all code necessary to clean, transform, and curate datasets for analysis.</li>
    <li><strong>Raw Datasets:</strong> Contains all original datasets used in the project.</li>
    <li><strong>Cleaned Datasets:</strong> Contains the outputs after data cleaning.</li>
</ul>

<h2>How to Use</h2>
<ol>
    <li>Download the <strong>Raw Datasets</strong> folder.</li>
    <li>Download the <strong>Code</strong> to the same folder.</li>
    <li>Execute the code in the following order:
        <ol class="instructions">
            <li>Passenger_Employee_Ratio_Code</li>
            <li>Webscrape_MIT</li>
            <li>delayed_data_MB</li>
            <li>Allen_Data_Cleaning</li>
            <li>omni_data_creation</li>
            <li>SerpApi_Compiled_Scrape</li>
        </ol>
    </li>
</ol>

<h2>Data Overview</h2>

<h3>Baggage</h3>
<ul class="data-description">
    <li><strong>Original file:</strong> 'Commercial_Aviation_Mishandled_Baggage.csv'</li>
    <li><strong>Source:</strong> <a href="https://data.bts.gov/Aviation/Commercial-Aviation-Mishandled-Baggage-and-Mishand/6u8d-47ih/about_data" target="_blank">BTS Data Source</a></li>
    <li><strong>Cleaned file:</strong> 'Baggage_Base_Data_Cleaned.csv'</li>
    <li><strong>Description:</strong> Contains carriers, mishandled baggage, total baggage, and mishandle rates. "Mishandled" refers to bags that encountered issues during the flight process.</li>
</ul>

<h3>Wages</h3>
<ul class="data-description">
    <li><strong>Original files:</strong> 'Average Annual Wages and Salaries - All Employees.csv', 'Average Annual Wages and Salaries - All Non-Cockpit Employees.csv'</li>
    <li><strong>Cleaned files:</strong> 'All_Wages.csv', 'Attend_Wages.csv', 'Handling_Wages.csv', 'Maint_Wages.csv', 'Pilot_Wages.csv'</li>
    <li><strong>Source:</strong> <a href="https://web.mit.edu/airlinedata/www/Employees&Compensation.html" target="_blank">MIT Airline Data</a></li>
    <li><strong>Description:</strong> Contains categories of wages, carrier information, and average salaries per year.</li>
</ul>

<h3>IATA Codes</h3>
<ul class="data-description">
    <li><strong>File name:</strong> 'US_iata_codes.csv'</li>
    <li><strong>Source:</strong> <a href="https://datahub.io/core/airport-codes#pandas" target="_blank">DataHub</a></li>
    <li><strong>Description:</strong> Contains U.S. airport names, states, IATA codes, latitude, and longitude.</li>
</ul>

<h3>Net Income</h3>
<ul class="data-description">
    <li><strong>File name:</strong> 'net_income.csv'</li>
    <li><strong>Cleaned file:</strong> 'modified_income_data.csv'</li>
    <li><strong>Source:</strong> <a href="https://web.mit.edu/airlinedata/www/2020%2012%20Month%20Documents/Profitability,%20Balance%20Sheet%20&%20Cash%20Flow/Income%20Statement/Net%20Income%20(Loss).htm" target="_blank">MIT Airline Data</a></li>
    <li><strong>Description:</strong> Net income data for 15 airlines from 2000 to 2020.</li>
</ul>

<h3>Passengers</h3>
<ul class="data-description">
    <li><strong>File name:</strong> 'passengers.csv'</li>
    <li><strong>Cleaned file:</strong> 'modified_peeps_data.csv'</li>
    <li><strong>Source:</strong> <a href="https://web.mit.edu/airlinedata/www/2020%2012%20Month%20Documents/Traffic%20and%20Capacity/System%20Total/System%20Total%20Enplaned%20Passengers.htm" target="_blank">MIT Airline Data</a></li>
    <li><strong>Description:</strong> Enplaned passengers for 15 airlines from 1995 to 2020.</li>
</ul>

<h3>Revenue Passenger Miles (RPMs)</h3>
<ul class="data-description">
    <li><strong>File name:</strong> 'rpms.csv'</li>
    <li><strong>Cleaned file:</strong> 'modified_rpms_data.csv'</li>
    <li><strong>Source:</strong> <a href="https://web.mit.edu/airlinedata/www/2020%2012%20Month%20Documents/Traffic%20and%20Capacity/System%20Total/Total%20System%20Revenue%20Passenger%20Miles.htm" target="_blank">MIT Airline Data</a></li>
    <li><strong>Description:</strong> Revenue data for each mile a passenger flew from 1995 to 2020.</li>
</ul>

<h3>Passenger to Employee Ratio</h3>
<ul class="data-description">
    <li><strong>Source:</strong> <a href="https://web.mit.edu/airlinedata/www/Employees&Productivity.html" target="_blank">MIT Airline Data</a></li>
    <li><strong>Cleaned file:</strong> 'passenger_employee_ratio_cleaned.csv'</li>
    <li><strong>Description:</strong> Passenger to employee ratio data by airline and year.</li>
</ul>

<h3>Delayed Flight Data (2009-2019)</h3>
<ul class="data-description">
    <li><strong>File name:</strong> 'Airline_Delay_Cause.csv'</li>
    <li><strong>Cleaned file:</strong> 'delays_cleaned_MB.csv'</li>
    <li><strong>Source:</strong> <a href="https://www.transtats.bts.gov/ot_delay/OT_DelayCause1.asp?20=E" target="_blank">BTS Data</a></li>
    <li><strong>Description:</strong> Contains delay data aggregated by airline and airport for a specific month.</li>
</ul>

<h2>Code Instructions</h2>

<h3>Web Scraping for Passenger to Employee Ratio</h3>
<ul class="code-instructions">
    <li><strong>File name:</strong> 'Passenger_Employee_Ratio_code.ipynb'</li>
    <li><strong>Instructions:</strong> Run the notebook to generate 'Passenger_Employee_Ratio_cleaned.csv'.</li>
</ul>

<h3>Delayed Data Creation</h3>
<ul class="code-instructions">
    <li><strong>File name:</strong> 'delayed_data_MB.ipynb'</li>
    <li><strong>Instructions:</strong> Run the notebook to output '

