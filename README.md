# ci-paging-bootstrap-4
codeigniter style pagination with bootstrap 4
Original code : https://github.com/zulacom/ci-paging-bootstrap-4

copy <b>pagination.php</b> to <code>application/config/</code>

for more detail <a href="http://www.luthfiabdulazis.com/blog/post/codeigniter-pagination-style-with-bootstrap-4" target="_blank">read here</a>


Added font-awesome 5 Icons
Include <link href="https://use.fontawesome.com/releases/v5.0.2/css/all.css" rel="stylesheet"> in your webpage.


To test the functionality.Use this part in you controller.
- change the base_url 
- change teh view name

$this->load->library('pagination');
$config['base_url'] = '';
$config['total_rows'] = 200;
$config['per_page'] = 20;
$this->pagination->initialize($config);
$data = $this->pagination->create_links();
$this->load->view('some_view', $data);









