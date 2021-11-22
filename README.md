# changes


extesion 

extension UIImage {
    func resizeTopAlignedToFill(newWidth: CGFloat) -> UIImage? {
        let newHeight = size.height * newWidth / size.width
        let newSize = CGSize(width: newWidth, height: newHeight)
        UIGraphicsBeginImageContextWithOptions(newSize, false, UIScreen.main.scale)
        draw(in: CGRect(origin: .zero, size: newSize))
        let newImage = UIGraphicsGetImageFromCurrentImageContext()
        UIGraphicsEndImageContext()
        return newImage
    }
}

DWCrpHomeScreenViewController

func prepareUI() {
        btnTakeRiskProfile.isEnabled = false
        imgTopBackground.layoutIfNeeded()
        imgBackground.layoutIfNeeded()
        let image = DWDashboardResources.image(name: DWDashboardResources.assets?.crpBackground).resizeTopAlignedToFill(newWidth: imgBackground.frame.size.width)
        imgTopBackground.image = image
        imgBackground.image = image
        btnTakeRiskProfile.setTitle(DWDashboardResources.copy?.buttonTakeCRP, for: .normal)
    }
    func prepareHeaderView() {
        self.navigationController?.navigationBar.isHidden = true
        lblHeaderTitle.font = CDFont.HeaderLarge
        lblHeaderTitle.textColor = CDColor.Palette.white
        lblHeaderTitle.isHidden = false
        let title = DWDashboardResources.copy?.screenheaderMeasuringRiskAppetite
        lblHeaderTitle.text = title
        lblHeaderTitleSmall.font = CDFont.HeaderSmall
        lblHeaderTitleSmall.textColor = CDColor.Palette.white
        lblHeaderTitleSmall.isHidden = true
        lblHeaderTitleSmall.text = title
        stickyHeaderView.backgroundColor = CDColor.Palette.transparent
        topBarView.backgroundColor = stickyHeaderView.backgroundColor
        headerBtnBack.setImage(DWDashboardResources.image(name: DWDashboardResources.assets?.iconBack), for: .normal)
        self.lblHeaderTitle.sizeToFit()
        headerViewInitialHeight = self.lblHeaderTitle.bounds.size.height + self.headerBtnBack.frame.origin.y + self.headerBtnBack.bounds.size.height + CDSpace.xxs
        setupHeaderForExpandedState()
    }
    
    DWAssessmentCompletedContainerViewController
    
    func prepareHeaderView() {
        lblHeaderTitle.font = CDFont.HeaderLarge
        lblHeaderTitle.textColor = self.headerTitleColor
        lblHeaderTitle.isHidden = false
        lblHeaderTitle.text = headerTitle
        lblHeaderTitleSmall.font = CDFont.HeaderSmall
        lblHeaderTitleSmall.textColor = self.headerTitleColor
        lblHeaderTitleSmall.isHidden = true
        lblHeaderTitleSmall.text = headerTitle
        stickyHeaderView.backgroundColor = CDColor.Palette.transparent
        topBarView.backgroundColor = stickyHeaderView.backgroundColor
        imgTopBackground.layoutIfNeeded()
        imgBackground.layoutIfNeeded()
        let image = DWDashboardResources.image(name: DWDashboardResources.assets?.crpPatternBG).resizeTopAlignedToFill(newWidth: imgBackground.frame.size.width)
        imgTopBackground.image = image
        imgBackground.image = image
        headerBtnBack.setImage(DWDashboardResources.image(name: DWDashboardResources.assets?.iconBack), for: .normal)
        self.lblHeaderTitle.sizeToFit()
        headerViewInitialHeight = self.lblHeaderTitle.bounds.size.height + self.headerBtnBack.frame.origin.y + self.headerBtnBack.bounds.size.height + CDSpace.s + CDSpace.xxs
        setupHeaderForExpandedState()
    }
    
    DWLossToleranceContainerViewController
    
    func prepareHeaderView() {
        btnPrimary.isEnabled = false
        self.navigationController?.navigationBar.isHidden = true
        btnPrimary.setTitle(buttonTitle, for: .normal)
        lblHeaderTitle.font = CDFont.HeaderLarge
        lblHeaderTitle.textColor = self.headerTitleColor
        lblHeaderTitle.isHidden = false
        lblHeaderTitle.text = headerTitle
        lblHeaderTitleSmall.font = CDFont.HeaderSmall
        lblHeaderTitleSmall.textColor = self.headerTitleColor
        lblHeaderTitleSmall.isHidden = true
        lblHeaderTitleSmall.text = headerTitle
        stickyHeaderView.backgroundColor = CDColor.Palette.white
        topBarView.backgroundColor = stickyHeaderView.backgroundColor
        imgNavSeprator.backgroundColor = CDColor.Palette.greyLightest
        headerBtnBack.setImage(DWDashboardResources.image(name: DWDashboardResources.assets?.iconBackBlue), for: .normal)
        self.lblHeaderTitle.sizeToFit()
        headerViewInitialHeight = self.lblHeaderTitle.bounds.size.height + self.headerBtnBack.frame.origin.y + self.headerBtnBack.bounds.size.height + CDSpace.xs
        setupHeaderForExpandedState()
    }
    
    DWMarketDownturnContainerViewController
    
    func prepareHeaderView() {
        btnPrimary.isEnabled = false
        self.navigationController?.navigationBar.isHidden = true
        btnPrimary.setTitle(buttonTitle, for: .normal)
        lblHeaderTitle.font = CDFont.HeaderLarge
        lblHeaderTitle.textColor = self.headerTitleColor
        lblHeaderTitle.isHidden = false
        lblHeaderTitle.text = headerTitle
        lblHeaderTitleSmall.font = CDFont.HeaderSmall
        lblHeaderTitleSmall.textColor = self.headerTitleColor
        lblHeaderTitleSmall.isHidden = true
        lblHeaderTitleSmall.text = headerTitle
        stickyHeaderView.backgroundColor = CDColor.Palette.white
        topBarView.backgroundColor = stickyHeaderView.backgroundColor
        imgNavSeprator.backgroundColor = CDColor.Palette.greyLightest
        headerBtnBack.setImage(DWDashboardResources.image(name: DWDashboardResources.assets?.iconBackBlue), for: .normal)
        self.lblHeaderTitle.sizeToFit()
        headerViewInitialHeight = self.lblHeaderTitle.bounds.size.height + self.headerBtnBack.frame.origin.y + self.headerBtnBack.bounds.size.height + CDSpace.xs
        setupHeaderForExpandedState()
    }
    
    DWCommonHeaderViewController
    
    func prepareHeaderView() {
        btnPrimary.isEnabled = false
        self.navigationController?.navigationBar.isHidden = true
        btnPrimary.setTitle(buttonTitle, for: .normal)
        lblHeaderTitle.font = CDFont.HeaderLarge
        lblHeaderTitle.textColor = self.headerTitleColor
        lblHeaderTitle.isHidden = false
        lblHeaderTitle.text = headerTitle
        lblHeaderTitleSmall.font = CDFont.HeaderSmall
        lblHeaderTitleSmall.textColor = self.headerTitleColor
        lblHeaderTitleSmall.isHidden = true
        lblHeaderTitleSmall.text = headerTitle
        stickyHeaderView.backgroundColor = CDColor.Palette.white
        topBarView.backgroundColor = stickyHeaderView.backgroundColor
        imgNavSeprator.backgroundColor = CDColor.Palette.greyLightest
        headerBtnBack.setImage(DWDashboardResources.image(name: DWDashboardResources.assets?.iconBackBlue), for: .normal)
        self.lblHeaderTitle.sizeToFit()
        headerViewInitialHeight = self.lblHeaderTitle.bounds.size.height + self.headerBtnBack.frame.origin.y + self.headerBtnBack.bounds.size.height + CDSpace.xs
        setupHeaderForExpandedState()
    }
