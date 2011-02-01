            * Oracle DB Monitor ZenPack Usage Notes *

Check INSTALL.txt for installation notes.

1. Features
   The Oracle DB Monitor ZenPack is a basic monitoring tool for Oracle database instances. It does not replace tools like Oracle Enterprise Manager nor does it aim to provide the same features.
   
   The aim here is to alert the DBA about problems that may occur or to give a general view on database performance and status, then other tools outside Zenoss can then be used to solve or drill-down on problems. 

   It has the following statistics/alerts:
      - To be completed.
   

. Using
   After installing the ZenPack according to instructions bind the Monitoring Template to your device and in the device configuration properties, fill out:
   - zOracleDBUsername - Your Oracle DB monitoring username with SELECT_CATALOG role (default dbsnmp).
   - zOracleDBPassword - Password for above.
   - zOracleDBCnxString - The connection string as configured on your tnsnames.ora.
   

. Known Problems
   - Errors in zenhub.log related to derived thresholds
      When adding the template to a new device you may see errors like:
      
      pythonThresholdException: User-supplied Python expression (here.getRRDValue('MaxProcesses')*0.9) for maximum value caused error: ['OracleRESOURCE_CurrProcesses']
      
      These errors are normal and can be ignored, after about 15-30 minutes they should disappear.
      

. Contact
   You may use the Issues feature at GitHub to log any problems or feature requests you may have.
   
   http://github.com/pmrpla/ZenPacks.community.OracleDBMon

   This is not a full time project so I will deal with your requests as best as I can.
   

. License
    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.
