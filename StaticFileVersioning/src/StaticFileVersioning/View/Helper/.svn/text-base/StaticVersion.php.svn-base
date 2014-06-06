<?php
namespace StaticFileVersioning\View\Helper;
use Zend\View\Helper\AbstractHelper;

class StaticVersion extends AbstractHelper {
    public function __invoke($path,$prefix = '?v=',$suffix = '') {
		 $version = filemtime('..'.$path);
		 $version = md5($version);
		 return $path . $prefix . $version . $suffix;
    }
}
