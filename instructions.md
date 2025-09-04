# Instructions

## Changing banner / header
* modify :
* Options:

  * Set the link (href)
  
  If you want the header to just reload your homepage, use:
  
  <a href="{{ '/' | relative_url }}">
    <img src="{{ '/assets/images/header.jpg' | relative_url }}" alt="Header Image">
  </a>
  
  
  If you want it to link to your institute page, replace with your real URL:
  
  <a href="https://icm.csic.es" target="_blank">
    <img src="{{ '/assets/images/header.jpg' | relative_url }}" alt="Header Image">
  </a>

  * Optional: make it configurable via _config.yml
  If you’d rather not hard-code it, you can replace with:
  
  <a href="{{ site.header.link | default: '/' | relative_url }}">
    <img src="{{ site.header.image | relative_url }}" alt="Header Image">
  </a>
  
  
  Then in your _config.yml you’d set:
  
  header:
    image: /assets/images/my-banner.jpg
    link: https://icm.csic.es
