# notes
onSecondGridReady(params) {
    const agBodyViewport: HTMLElement = this.elementRef.nativeElement.querySelector('#secondGrid .ag-body-viewport');
    const agBodyHorizontalViewport: HTMLElement = this.elementRef.nativeElement.querySelector('#secondGrid .ag-body-horizontal-scroll-viewport');
    if (agBodyViewport) {
      const ps = new PerfectScrollbar(agBodyViewport);
      ps.update();
    }
    if (agBodyHorizontalViewport) {
      const ps = new PerfectScrollbar(agBodyHorizontalViewport);
      ps.update();
    }
  }
  
  .container {
  display: flex;
}

#FirstGrid .ag-body-viewport {
  position: relative;
  overflow: hidden !important;
}

#secondGrid .ag-body-viewport,
#secondGrid .ag-body-horizontal-scroll-viewport {
  position: relative;
  overflow: hidden !important;
}

.ps__rail-x,
.ps__rail-y {
  opacity: 0.6;
}
