```python
import pandas as pd
```


```python
issueFile = pd.read_excel('Downloads/airIssues.xlsx')

issueFile
```




<div>

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>ID</th>
      <th>Start time</th>
      <th>Completion time</th>
      <th>Email</th>
      <th>Name</th>
      <th>Last modified time</th>
      <th>Airline</th>
      <th>Issue Details\n</th>
      <th>URL\n</th>
      <th>Browser</th>
      <th>Last checked on\n</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>2024-12-07 17:53:16</td>
      <td>2024-12-07 17:53:53</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>KLM</td>
      <td>Often searching for a flight leads to an indef...</td>
      <td>https://www.klm.co.id/search/flights/0</td>
      <td>Firefox</td>
      <td>2024-12-07</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>2024-12-07 17:54:47</td>
      <td>2024-12-07 18:10:54</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>KLM</td>
      <td>After searching for a flight once, if you make...</td>
      <td>https://www.klm.com/search/flights/0</td>
      <td>Firefox</td>
      <td>2024-12-07</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>2024-12-07 18:12:15</td>
      <td>2024-12-07 18:13:19</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>KLM</td>
      <td>Same lies about (x seats left). When you open ...</td>
      <td>NaN</td>
      <td>Firefox</td>
      <td>2024-12-07</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4</td>
      <td>2024-12-07 18:30:57</td>
      <td>2024-12-07 18:31:20</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>KLM</td>
      <td>Unsure if its their Indonesia website only but...</td>
      <td>NaN</td>
      <td>Firefox</td>
      <td>2024-12-07</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5</td>
      <td>2024-12-09 23:59:11</td>
      <td>2024-12-10 10:57:26</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Singapore Airlines</td>
      <td>"Please note the following operating hours for...</td>
      <td>https://www.singaporeair.com/en_UK/sg/travel-i...</td>
      <td>Firefox</td>
      <td>2024-12-09</td>
    </tr>
    <tr>
      <th>5</th>
      <td>6</td>
      <td>2024-12-14 14:53:34</td>
      <td>2024-12-14 19:09:45</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Batik Air</td>
      <td>On home page, while selecting the date, the mo...</td>
      <td>https://www.batikair.com.my</td>
      <td>Firefox</td>
      <td>2024-12-14</td>
    </tr>
    <tr>
      <th>6</th>
      <td>7</td>
      <td>2024-12-15 16:47:04</td>
      <td>2024-12-15 23:46:21</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Singapore Airlines</td>
      <td>On clicking the fare type pop-up, it doesn't c...</td>
      <td>https://www.singaporeair.com/en_UK/us/travel-i...</td>
      <td>Firefox</td>
      <td>2024-12-15</td>
    </tr>
    <tr>
      <th>7</th>
      <td>8</td>
      <td>2024-12-17 11:22:30</td>
      <td>2024-12-17 11:40:58</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Qatar</td>
      <td>When you open the help (customer support chat)...</td>
      <td>https://www.qatarairways.com/en/Privilege-Club...</td>
      <td>Safari</td>
      <td>2024-12-17</td>
    </tr>
    <tr>
      <th>8</th>
      <td>9</td>
      <td>2024-12-20 09:26:48</td>
      <td>2024-12-20 09:36:55</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Singapore Airlines</td>
      <td>When going on your homepage's top to see notif...</td>
      <td>https://www.singaporeair.com/en_UK/us/home#/bo...</td>
      <td>Safari</td>
      <td>2024-12-20</td>
    </tr>
    <tr>
      <th>9</th>
      <td>10</td>
      <td>2024-12-21 07:47:23</td>
      <td>2024-12-21 09:39:36</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Singapore Airlines</td>
      <td>Entering SIN (mostly intended for Singapore as...</td>
      <td>https://www.singaporeair.com/flightsearch/sear...</td>
      <td>Safari</td>
      <td>2024-12-21</td>
    </tr>
    <tr>
      <th>10</th>
      <td>11</td>
      <td>2024-12-26 16:46:55</td>
      <td>2024-12-27 21:36:10</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Qatar</td>
      <td>Whenever we select the "upper deck" seats for ...</td>
      <td>N/A (App issue)</td>
      <td>Internet Explorer</td>
      <td>2024-12-26</td>
    </tr>
    <tr>
      <th>11</th>
      <td>12</td>
      <td>2025-01-09 09:35:50</td>
      <td>2025-01-09 10:59:26</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Turkish</td>
      <td>When selecting a stopover in Istanbul, it does...</td>
      <td>https://www.turkishairlines.com/en-int/flights...</td>
      <td>Safari</td>
      <td>2025-01-09</td>
    </tr>
    <tr>
      <th>12</th>
      <td>13</td>
      <td>2025-01-13 09:06:19</td>
      <td>2025-01-14 01:16:54</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Singapore Airlines</td>
      <td>Career Page shows a minor error (Singapore for...</td>
      <td>https://www.singaporeair.com/en_UK/sg/careers/...</td>
      <td>Firefox</td>
      <td>2025-01-13</td>
    </tr>
    <tr>
      <th>13</th>
      <td>14</td>
      <td>2025-01-17 07:21:38</td>
      <td>2025-01-18 00:13:41</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Bangkok Airways</td>
      <td>When selecting multicity trip, second flight's...</td>
      <td>https://www.bangkokair.com</td>
      <td>Safari</td>
      <td>2025-01-17</td>
    </tr>
    <tr>
      <th>14</th>
      <td>15</td>
      <td>2025-01-24 08:36:40</td>
      <td>2025-01-24 10:23:12</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Qatar Airways</td>
      <td>While selecting stopover (from front page), wh...</td>
      <td>https://www.qatarairways.com/en-pk/homepage.html</td>
      <td>Safari</td>
      <td>2025-01-24</td>
    </tr>
    <tr>
      <th>15</th>
      <td>16</td>
      <td>2025-01-26 10:43:26</td>
      <td>2025-01-26 10:45:09</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>SIA</td>
      <td>Book Now" link on Singapore Tour takes to an e...</td>
      <td>https://isolate.menlosecurity.com/readonly/htt...</td>
      <td>Safari</td>
      <td>2025-01-26</td>
    </tr>
    <tr>
      <th>16</th>
      <td>17</td>
      <td>2025-01-27 00:25:38</td>
      <td>2025-01-27 00:43:47</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>SIA</td>
      <td>Multi-city search isn't working for some time</td>
      <td>https://www.singaporeair.com/flightsearch/mult...</td>
      <td>Firefox</td>
      <td>2025-01-27</td>
    </tr>
    <tr>
      <th>17</th>
      <td>18</td>
      <td>2025-02-18 13:55:50</td>
      <td>2025-02-18 13:57:35</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Cathay Pacific</td>
      <td>Often it gets stuck and doesn't let select the...</td>
      <td>https://book.cathaypacific.com/CathayPacificV3...</td>
      <td>Safari</td>
      <td>2025-02-18</td>
    </tr>
    <tr>
      <th>18</th>
      <td>19</td>
      <td>2025-02-18 13:58:40</td>
      <td>2025-02-18 13:59:06</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Cathay Pacific</td>
      <td>Often booking search results in error</td>
      <td>https://book.cathaypacific.com/CathayPacificV3...</td>
      <td>Safari</td>
      <td>2025-02-18</td>
    </tr>
    <tr>
      <th>19</th>
      <td>20</td>
      <td>2025-02-24 06:41:44</td>
      <td>2025-02-24 13:08:35</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Cathay Pacific</td>
      <td>During multi-city search, if you select two fl...</td>
      <td>https://book.cathaypacific.com/CathayPacificV3...</td>
      <td>Safari</td>
      <td>2025-02-24</td>
    </tr>
    <tr>
      <th>20</th>
      <td>21</td>
      <td>2025-02-26 07:28:41</td>
      <td>2025-02-26 09:01:21</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Cathay Pacific</td>
      <td>Applying the filters doesn't work. It still sh...</td>
      <td>https://book.cathaypacific.com/CathayPacificV3...</td>
      <td>Safari</td>
      <td>2025-02-26</td>
    </tr>
    <tr>
      <th>21</th>
      <td>22</td>
      <td>2025-03-05 08:49:02</td>
      <td>2025-03-06 13:15:56</td>
      <td>anonymous</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Cathay Pacific</td>
      <td>When sorting the search results by "Fare", it ...</td>
      <td>https://book.cathaypacific.com/CathayPacificV3...</td>
      <td>Safari</td>
      <td>2025-03-05</td>
    </tr>
  </tbody>
</table>
</div>




```python

```
