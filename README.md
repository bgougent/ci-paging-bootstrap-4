# ci-paging-bootstrap-4
codeigniter style pagination with bootstrap 4
Original code : https://github.com/zulacom/ci-paging-bootstrap-4

copy <b>pagination.php</b> to <code>application/config/</code>

<b>Added font-awesome 5 Icons</b><br/>
Include <a href="https://use.fontawesome.com/releases/v5.0.2/css/all.css" target="_blank" >href="https://use.fontawesome.com/releases/v5.0.2/css/all.css"</a> as style in your webpage.


To test the functionality.Use this part in you controller.
- change the base_url 
- change teh view name
<pre><code>$this->load->library('pagination'); 
$config['base_url'] = '';
$config['total_rows'] = 200;
$config['per_page'] = 20;
$this->pagination->initialize($config);
$data = $this->pagination->create_links();
$this->load->view('some_view', $data);
</code></pre>








