## [Download an Active or Archived Recording](#download-an-active-or-archived-recording)
Cryostat provides some in-cluster online Flight Recording analysis tools, but
the heavy lifting of JFR analysis workflows is still done using
[JDK Mission Control](https://github.com/openjdk/jmc). The easiest way to do
this is to get a copy of a JFR binary file on your local workstation and open
it with JMC from there. This is the core feature of Cryostat - creating Flight
Recordings in your containerized JVMS, and retrieving that data to developers'
and admins' local workstations.

<ol>
  <li>
    <details>
      <summary>Select the target application</summary>
      <a href="{{site.url}}/images/download-an-active-or-archived-recording-1.png" target="_blank">
        <img src="{{site.url}}/images/download-an-active-or-archived-recording-1.png">
      </a>
    </details>
  </li>
  <li>
    <details>
      <summary>Navigate to Recordings</summary>
      <a href="{{site.url}}/images/download-an-active-or-archived-recording-2.png" target="_blank">
        <img src="{{site.url}}/images/download-an-active-or-archived-recording-2.png">
      </a>
      <p>
        Supply JMX credentials to authenticate to the target, if necessary. If
        the target is not configured with JMX authentication then the
        connection attempt will continue without prompting for credentials.
      </p>
      <p>
        If the target JVM has SSL/TLS enabled on JMX connections then it may be
        necessary to add the target's certificate to Cryostat's trust store. Go
        to <a href="{{site.url}}/getting-started#add-a-trusted-certificate">Add a Trusted Certificate</a>
        and return to this section after completing that guide.
      </p>
      <a href="{{site.url}}/images/download-an-active-or-archived-recording-3.png" target="_blank">
        <img src="{{site.url}}/images/download-an-active-or-archived-recording-3.png">
      </a>
    </details>
  </li>
</ol>
